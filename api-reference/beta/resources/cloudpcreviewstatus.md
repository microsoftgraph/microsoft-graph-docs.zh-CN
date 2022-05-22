---
title: cloudPcReviewStatus 资源类型
description: 表示有关云电脑的审阅状态的详细信息。
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: efaaeeab9474ab785cba4f40e64794af6d3344fc
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629498"
---
# <a name="cloudpcreviewstatus-resource-type"></a>cloudPcReviewStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关云电脑的审阅状态的详细信息。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|azureStorageAccountId|String|保存云电脑快照的Azure 存储帐户的资源 ID。|
|azureStorageAccountName|String|保存云电脑快照的Azure 存储帐户的名称。|
|inReview|Boolean| `True` 如果管理员将云电脑设置为正在查看。|
|restorePointDateTime|DateTimeOffset|云电脑快照的特定日期和时间，当云电脑设置为审阅时自动创建和保存。 时间戳以 ISO 8601 格式显示，协调世界时 (UTC) 。 例如，2014 年 1 月 1 日午夜 UTC 显示为 `2014-01-01T00:00:00Z`。|
|reviewStartDateTime|DateTimeOffset|云电脑设置为审阅的特定日期和时间。 时间戳以 ISO 8601 格式显示，协调世界时 (UTC) 。 例如，2014 年 1 月 1 日午夜 UTC 显示为 `2014-01-01T00:00:00Z`。|
|subscriptionId|String|保存云电脑快照的 Azure 订阅的 ID，格式为 GUID。|
|subscriptionName|字符串|保存云电脑快照的 Azure 订阅的名称。|
|userAccessLevel|[cloudPcUserAccessLevel](#cloudpcuseraccesslevel-values)|云电脑上最终用户的访问级别。 可取值为：`unrestricted`、`restricted`。|

### <a name="cloudpcuseraccesslevel-values"></a>cloudPcUserAccessLevel 值

|成员|值|Description|
|:---|:---|:---|
|unrestricted|0|无限制。 用户可以访问云电脑。|
|限制|1|不允许用户访问云电脑。|
|unknownFutureValue|999|可变枚举 sentinel 值。 请勿使用。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcReviewStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcReviewStatus",
  "azureStorageAccountId": "String",
  "azureStorageAccountName": "String",
  "inReview": "Boolean",
  "restorePointDateTime": "String (timestamp)",
  "reviewStartDateTime": "String (timestamp)",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "userAccessLevel": "String"
}
```

