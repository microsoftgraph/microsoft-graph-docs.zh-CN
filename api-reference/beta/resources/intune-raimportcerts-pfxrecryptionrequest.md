---
title: pfxRecryptionRequest 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7accd07576b93448268eed950768b02a57eceb68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074848"
---
# <a name="pfxrecryptionrequest-resource-type"></a>pfxRecryptionRequest 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 pfxRecryptionRequests](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 集合|列出 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象的属性和关系。|
|[Get pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|读取 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象的属性和关系。|
|[创建 pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|创建新的 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象。|
|[删除 pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|无|删除 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)。|
|[更新 pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|更新 [pfxRecryptionRequest 对象](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|tenantId|Guid|尚未记录|
|userId|Guid|尚未记录|
|deviceId|Guid|尚未记录|
|profileId|Guid|尚未记录|
|thumbprint|String|尚未记录|
|deviceKeyThumbprint|String|尚未记录|
|status|Int32|尚未记录|
|sourceType|Int32|尚未记录|
|createdTime|DateTimeOffset|尚未记录|
|lastModifiedTime|DateTimeOffset|尚未记录|
|isDeleted|Boolean|尚未记录|
|eTag|String|尚未记录|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxRecryptionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "profileId": "Guid",
  "thumbprint": "String",
  "deviceKeyThumbprint": "String",
  "status": 1024,
  "sourceType": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "isDeleted": true,
  "eTag": "String"
}
```



