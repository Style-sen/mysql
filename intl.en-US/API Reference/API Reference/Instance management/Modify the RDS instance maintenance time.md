# Modify the RDS instance maintenance time {#reference_gx3_2cf_12b .reference}

## Description {#section_l21_v32_12b .section}

Modify the time for routine instance maintenance. You can set a period of time during which traffic is low. Alibaba Cloud performs routine maintenance within the maintenance period you have set so as to minimize impacts on your services.

## Request parameters {#section_qzx_w32_12b .section}

|Name|Type|Required?|Description|
|----|----|---------|-----------|
|Action|String|Yes|Required parameter. Value: ModifyDBInstanceMaintainTime.|
|DBInstanceId|String|Yes|Instance ID.|
|MaintainTime|String|Yes|Instance maintenance time. Value options:-   22:00Z-02:00Z: 10:00 pm to 02:00 am
-   02:00Z-06:00Z: 02:00 am to 06:00 am
-   06:00-10:00: 6:00 am to 10:00 am
-   10:00Z-14:00Z: 10:00 am to 02:00 pm
-   14:00Z-18:00Z: 02:00 pm to 06:00 pm
-   18:00Z-22:00Z: 06:00 pm to 10:00 pm

|

## Return parameters {#section_rpk_z32_12b .section}

|Name|Type|Description|
|----|----|-----------|
|<Public Return Parameters\>|-|For more information, see [Public parameters](intl.en-US/API Reference/Use APIs/Public parameters.md#).|

## Request example {#section_l4g_pj2_12b .section}

```
https://rds.aliyuncs.com/?Action=ModifyDBInstanceMaintainTime
& Dbinstanceid = rdsaiiabnaiiabn
&MaintainTime=22:00Z-02:00Z
&<Public Request Parameters>
```

## Response example {#section_xtg_rj2_12b .section}

**XML format**

```
<ModifyDBInstanceMaintainTimeResponse>
         <RequestId>65BDA532-28AF-4122-AA39-B382721EEE64</RequestId>
</ModifyDBInstanceMaintainTimeResponse>
```

**JSON format**

```

    "RequestId": " 65BDA532-28AF-4122-AA39-B382721EEE64"
  
```

