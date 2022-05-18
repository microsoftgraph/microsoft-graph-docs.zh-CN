---
title: subjectRightsRequest 资源类型
description: 表示使用者权限请求的属性。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f59c1306bea22b0da7e59024600017e73dfa8eff
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461434"
---
# <a name="subjectrightsrequest-resource-type"></a>subjectRightsRequest 资源类型

命名空间：microsoft.graph

表示使用者权限请求的属性，这是受控制者要求对其个人数据执行操作的数据的正式请求。 

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 subjectRightsRequests](../api/subjectRightsRequest-list.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md) 集合|获取 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象及其属性的列表。|
|[创建 subjectRightsRequest](../api/subjectRightsRequest-post.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|创建新的 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象。|
|[获取 subjectRightsRequest](../api/subjectRightsRequest-get.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|读取 [subjectRightsRequest 对象的](../resources/subjectRightsRequest.md) 属性和关系。|
|[更新 subjectRightsRequest](../api/subjectRightsRequest-update.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|更新 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象的属性。|
|[getFinalAttachment](../api/subjectRightsRequest-getfinalattachment.md)|Stream|获取请求的最后附件。 附件是一个 zip 文件，其中包含隐私管理员包含的所有文件。|
|[getFinalReport](../api/subjectRightsRequest-getfinalreport.md)|Stream|获取请求的最终报告。 报表是一个文本文件，其中包含隐私管理员包含的文件的相关信息。|
|[列出备注](../api/subjectRightsRequest-list-notes.md)|[authoredNote](../resources/authorednote.md) 集合|从备注导航属性获取 authoredNote 资源。|
|[创建 authoredNote](../api/subjectRightsRequest-post-notes.md)|[authoredNote](../resources/authorednote.md)|创建新的 authoredNote 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedTo|[identity](../resources/identity.md)|将请求分配给的标识。|
|closedDateTime|DateTimeOffset|请求关闭的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|createdBy|[identitySet](../resources/identityset.md)|创建请求的实体的标识信息。|
|createdDateTime|DateTimeOffset|创建请求的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
|dataSubject|[dataSubject](../resources/datasubject.md)|有关数据主题的信息。|
|dataSubjectType|dataSubjectType|数据主体的类型。 可取值为：`customer`、`currentEmployee`、`formerEmployee`、`prospectiveEmployee`、`student`、`teacher`、`faculty`、`other`、`unknownFutureValue`。|
|说明|String|请求的说明。|
|displayName|String|请求的名称。|
|历史|[subjectRightsRequestHistory](../resources/subjectRightsRequesthistory.md) 集合|历史记录更改事件的集合。|
|洞察 力|[subjectRightsRequestDetail](../resources/subjectRightsRequestdetail.md)|有关请求的见解。|
|internalDueDateTime|DateTimeOffset|请求在内部到期的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改请求的实体的标识信息。|
|lastModifiedDateTime|DateTimeOffset|上次修改请求的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|法规|String collection|此请求将履行的法规列表。|
|stages|[subjectRightsRequestStageDetail](../resources/subjectRightsRequeststagedetail.md) 集合|有关请求的不同阶段的信息。|
|status|subjectRightsRequestStatus|请求的状态。 可取值为：`active`、`closed`、`unknownFutureValue`。|
|type|subjectRightsRequestType|请求的类型。 可能的值为： `export`， `delete`， `access`， `tagForAction`， 。 `unknownFutureValue`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|notes|[authoredNote](../resources/authorednote.md) 集合|随请求一起分配的备注列表。|
|团队|[团队](../resources/team.md)|有关为请求创建的Microsoft Teams团队的信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subjectRightsRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequest",
    "type": "access",
    "dataSubjectType": "customer",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String (timestamp)",
    "closedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "completed",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "contentReview",
            "status": "current",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": 
            {
                "@odata.type": "microsoft.graph.publicError"
            }
        }
    ],
    "insight": {
        "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
    },
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "@odata.type": "microsoft.graph.dataSubject",
    },
    "team": {
        "@odata.type": "microsoft.graph.team"
    }
}
```

