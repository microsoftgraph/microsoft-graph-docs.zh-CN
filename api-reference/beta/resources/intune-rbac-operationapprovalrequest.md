---
title: operationApprovalRequest 资源类型
description: OperationApprovalRequest 实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45c2b30a39c9930ee8a8d7def27a06e7617fddbf
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346743"
---
# <a name="operationapprovalrequest-resource-type"></a>operationApprovalRequest 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OperationApprovalRequest 实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List operationApprovalRequests](../api/intune-rbac-operationapprovalrequest-list.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 集合|列出 [operationApprovalRequest 对象的属性和](../resources/intune-rbac-operationapprovalrequest.md) 关系。|
|[获取 operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-get.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|读取 [operationApprovalRequest 对象的属性和](../resources/intune-rbac-operationapprovalrequest.md) 关系。|
|[创建 operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-create.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|创建新的 [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 对象。|
|[删除 operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-delete.md)|无|删除 [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)。|
|[Update operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-update.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|更新 [operationApprovalRequest 对象](../resources/intune-rbac-operationapprovalrequest.md) 的属性。|
|[审批操作](../api/intune-rbac-operationapprovalrequest-approve.md)|String|批准请求的操作实例ApprovalRequest|
|[拒绝操作](../api/intune-rbac-operationapprovalrequest-reject.md)|String|拒绝请求的 operationApprovalRequest 实例|
|[cancelApproval 操作](../api/intune-rbac-operationapprovalrequest-cancelapproval.md)|String|取消已批准的 operationApprovalRequest 实例|
|[getRequestStatus 操作](../api/intune-rbac-operationapprovalrequest-getrequeststatus.md)|[operationApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md)|尚未记录|
|[getMyRequestById 函数](../api/intune-rbac-operationapprovalrequest-getmyrequestbyid.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|尚未记录|
|[getMyRequests 函数](../api/intune-rbac-operationapprovalrequest-getmyrequests.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) 集合|尚未记录|
|[cancelMyRequest 操作](../api/intune-rbac-operationapprovalrequest-cancelmyrequest.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的 ID|
|requestDateTime|DateTimeOffset|请求的 DateTime。 此属性是只读的。|
|expirationDateTime|DateTimeOffset|不再允许对请求执行操作的日期/时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|上次修改日期时间。 此属性是只读的。|
|requestor|[identitySet](../resources/intune-rbac-identityset.md)|请求者的身份。 此属性是只读的。|
|审批者|[identitySet](../resources/intune-rbac-identityset.md)|审批者的身份。 此属性是只读的。|
|状态|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|当前审批请求状态。 此属性是只读的。 可取值为：`unknown`、`needsApproval`、`approved`、`rejected`、`cancelled`、`completed` 或 `expired`。|
|requestJustification|String|请求理由。 此属性是只读的。|
|approvalJustification|String|批准请求的理由。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "String (identifier)",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "status": "String",
  "requestJustification": "String",
  "approvalJustification": "String"
}
```




