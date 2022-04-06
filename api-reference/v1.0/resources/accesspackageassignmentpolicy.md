---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定主题可以通过访问包分配请求或分配访问包的策略。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 90f2b6024e63325a1e0c7e6d8156fa40189736b9
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608298"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>accessPackageAssignmentPolicy 资源类型

命名空间：microsoft.graph

在[Azure AD中](entitlementmanagement-overview.md)，访问包分配策略指定主题可以通过访问包分配请求或分配访问包的策略。 访问包可以具有零个或多个策略。 收到主题的请求时，将针对每个策略匹配主题，以查找包含该 () **requestorSettings** 的策略。 然后，该策略确定请求是否需要审批、访问包分配的持续时间，以及分配是否需要定期检查。

若要将用户分配给访问包，请创建引用访问包和访问包分配策略的 [accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) 。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 accessPackageAssignmentPolicies](../api/entitlementmanagement-list-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 集合|获取 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象及其属性的列表。|
|[创建 accessPackageAssignmentPolicy](../api/entitlementmanagement-post-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|创建新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。|
|[获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|读取 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的属性和关系。|
|[更新 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|更新 [accessPackageAssignmentPolicy 对象](../resources/accesspackageassignmentpolicy.md) 的属性。|
|[删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md)|无|删除 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|allowedTargetScope|allowedTargetScope|可以通过此策略分配访问包的主体。 可取值包括：`notSpecified`、`specificDirectoryUsers`、`specificConnectedOrganizationUsers`、`specificDirectoryServicePrincipals`、`allMemberUsers`、`allDirectoryUsers`、`allDirectoryServicePrincipals`、`allConfiguredConnectedOrganizationUsers`、`allExternalUsers`、`unknownFutureValue`。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|说明|String|策略的说明。|
|displayName|String|策略显示名称。|
|expiration|[expirationPattern](../resources/expirationpattern.md)|在此策略中创建的工作分配的到期日期。|
|id|String|只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|指定通过此策略审批访问包分配请求的设置。 例如，如果新请求需要审批。|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|提供其他设置，以选择谁可以通过此策略创建访问包分配请求，以及可以在请求中包括的内容。|
|reviewSettings|[accessPackageAssignmentReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|设置此策略访问分配评审。|
|specificAllowedTargets|[subjectSet](../resources/subjectset.md) 集合|可以通过此策略从访问包分配访问权限的主体。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|包含此策略的访问包。 只读。 |
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|包含此策略的访问包的目录。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "allowedTargetScope": "String",
  "specificAllowedTargets": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "requestorSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
  },
  "reviewSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
  },
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


