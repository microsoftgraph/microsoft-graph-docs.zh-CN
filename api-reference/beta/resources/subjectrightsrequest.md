---
title: subjectRightsRequest 资源类型
description: 表示主题权限请求的属性。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6aaa40989723309eb073c69aa22d53354bdbda7d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452101"
---
# <a name="subjectrightsrequest-resource-type"></a>subjectRightsRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示主体权限请求的属性，这是数据主体向控制者提出的对个人数据采取操作的正式请求。 

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 subjectRightsRequests](../api/subjectRightsRequest-list.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md) 集合|获取 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象及其属性的列表。|
|[创建 subjectRightsRequest](../api/subjectRightsRequest-post.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|创建新的 [subjectRightsRequest](../resources/subjectRightsRequest.md) 对象。|
|[获取 subjectRightsRequest](../api/subjectRightsRequest-get.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|读取 [subjectRightsRequest 对象的属性和](../resources/subjectRightsRequest.md) 关系。|
|[更新 subjectRightsRequest](../api/subjectRightsRequest-update.md)|[subjectRightsRequest](../resources/subjectRightsRequest.md)|更新 [subjectRightsRequest 对象](../resources/subjectRightsRequest.md) 的属性。|
|[getFinalAttachment](../api/subjectRightsRequest-getfinalattachment.md)|Stream|获取请求的最终附件。 附件是一个 zip 文件，其中包含隐私管理员包含的所有文件。|
|[getFinalReport](../api/subjectRightsRequest-getfinalreport.md)|Stream|获取请求的最终报告。 该报告是一个文本文件，其中包含隐私管理员包含的文件相关信息。|
|[列出注释](../api/subjectRightsRequest-list-notes.md)|[authoredNote](../resources/authorednote.md) 集合|从 notes 导航属性获取 authoredNote 资源。|
|[创建 authoredNote](../api/subjectRightsRequest-post-notes.md)|[authoredNote](../resources/authorednote.md)|创建新的 authoredNote 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedTo|[identity](../resources/identity.md)|请求分配到的标识。|
|closedDateTime|DateTimeOffset|关闭请求的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|createdBy|[identitySet](../resources/identityset.md)|创建请求的实体的标识信息。|
|createdDateTime|DateTimeOffset|创建请求的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
|dataSubject|[dataSubject](../resources/datasubject.md)|有关数据主体的信息。|
|dataSubjectType|dataSubjectType|数据主体的类型。 可取值为：`customer`、`currentEmployee`、`formerEmployee`、`prospectiveEmployee`、`student`、`teacher`、`faculty`、`other`、`unknownFutureValue`。|
|说明|String|请求的说明。|
|displayName|String|请求的名称。|
|history|[subjectRightsRequestHistory](../resources/subjectRightsRequesthistory.md) 集合|历史记录更改事件的集合。|
|insight|[subjectRightsRequestDetail](../resources/subjectRightsRequestdetail.md)|有关请求的见解。|
|internalDueDateTime|DateTimeOffset|请求在内部到期的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改请求的实体的标识信息。|
|lastModifiedDateTime|DateTimeOffset|上次修改请求的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|法规|String collection|此请求将履行的法规列表。|
|stages|[subjectRightsRequestStageDetail](../resources/subjectRightsRequeststagedetail.md) 集合|有关请求的不同阶段的信息。|
|status|subjectRightsRequestStatus|请求的状态。 可取值为：`active`、`closed`、`unknownFutureValue`。|
|type|subjectRightsRequestType|请求的类型。 可取值为：`export`、`delete`、`access`、`tagForAction`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|notes|[authoredNote](../resources/authorednote.md) 集合|与请求关联的注释列表。|
|团队|[团队](../resources/team.md)|有关为Microsoft Teams创建的团队的信息。|

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

