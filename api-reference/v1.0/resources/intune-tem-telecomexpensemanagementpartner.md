---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d083e9bd92cae588fdde7c29ac58c35e40a6bd2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021559"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>telecomExpenseManagementPartner 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List telecomExpenseManagementPartners](../api/intune-tem-telecomexpensemanagementpartner-list.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合|列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。|
|[Get telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。|
|[Create telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。|
|[Delete telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|无|删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。|
|[Update telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|TEM 合作伙伴的唯一标识符。|
|displayName|String|TEM 合作伙伴的显示名称。|
|url|String|TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。|
|appAuthorized|Boolean|是否已授权合作伙伴的 AAD 应用访问 Intune。|
|enabled|Boolean|当前是启用还是禁用了 Intune 的 TEM 服务连接。|
|lastConnectionDateTime|DateTimeOffset|TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```




