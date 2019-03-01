---
title: 域资源类型
description: 表示与租户相关联的域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b349920f0849ec18b0d5e70fda0bcb16c41e63c
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342329"
---
# <a name="domain-resource-type"></a>域资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与租户相关联的域。

使用域操作将域关联到租户，验证域所有关系并配置支持的服务。域操作让注册机构对服务（如 Office 365）的域关联启用自动化。例如，作为域注册的一部分，注册机构可以为电子邮件、网站、身份验证等启用虚域。

若要将域与租户相关联，请执行以下操作：

1. [关联](../api/domain-post-domains.md)域与租户。

2. [检索](../api/domain-list-verificationdnsrecords.md)域验证记录。使用域注册机构或 DNS 服务器配置，向域区域文件添加验证记录详细信息。

3. [验证](../api/domain-verify.md)域的所有权。这将验证域，并将 *isVerified* 属性设置为 *true*。

4. [指明](../api/domain-update.md)计划与域配合使用的受支持服务。

5. 通过检索需要为域启用服务的记录列表[配置](../api/domain-list-serviceconfigurationrecords.md)支持的服务。使用域注册机构或 DNS 服务器配置，向域区域文件添加配置记录详细信息。

## <a name="methods"></a>方法

| 方法   | 返回类型 |说明|
|:---------------|:--------|:----------|
|[获取域](../api/domain-get.md) | [domain](domain.md) | 读取 domain 对象的属性和关系。|
|[创建域](../api/domain-post-domains.md) | [domain](domain.md) | 向租户添加域。 |
|[列出 domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) collection| 通过对域的引用检索 directory 对象列表。|
|[列出 serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索域配置的域 DNS 记录列表。|
|[列出 verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索用于域验证的域 DNS 记录列表。|
|[更新域](../api/domain-update.md) | [domain](domain.md) |更新域。|
|[删除域](../api/domain-delete.md) | 无 |删除域。|
|[ForceDelete 域](../api/domain-forcedelete.md)|无|使用异步操作删除域。|
|[验证域](../api/domain-verify.md)|[域](domain.md)|验证域的所有权。|

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|authenticationType|String| 表示为域配置的身份验证类型。此为*托管*或*联盟*值。<br> *托管*表示 Azure AD 执行用户身份验证的云托管域。<br>*联盟*表示身份验证与标识提供程序（如通过 Active Directory 联合身份验证服务的租户的本地 Active Directory）联合。不可为 Null |
|availabilityStatus|String| 使用[验证](../api/domain-verify.md)操作时，此属性始终为 Null。使用[验证](../api/domain-verify.md)操作时，响应中返回**域**实体。响应中的**域**实体的 **availabilityStatus** 属性为 *AvailableImmediately* 或 *EmailVerifiedDomainTakeoverScheduled*。|
|id|字符串| 域的完全限定的名称。密钥、不可变、不可为 Null、唯一 |
|isAdminManaged|Boolean| 如果域的 DNS 记录管理已委派为 Office 365，则属性值为 false。否则，此值为 true。不可为 Null |
|isDefault|Boolean| 如果这是用于创建用户的默认域，则为 true。每个公司仅有一个默认域。不可为 Null |
|isInitial|Boolean| 如果这是由 Microsoft Online Services (companyname.onmicrosoft.com) 创建的初始域，则为 true。每个公司仅有一个初始域。不可为 Null |
|isRoot|Boolean| 如果此域是一个已验证的根域，则为 true。否则，如果此域为子域或未经验证，则为 false。不可为 Null |
|isVerified|Boolean| 如果域已完成域所有权验证，则为 true。不可为 Null |
|passwordNotificationWindowInDays|Int32|指定用户收到其密码将到期的通知之前的天数。 如果未设置该属性, 则将使用默认值14天。|
|passwordValidityPeriodInDays|Int32| 指定密码在必须更改之前有效的时间长度。 如果未设置该属性, 则将使用默认值90天。 |
|supportedServices|字符串集合| 分配给域的功能。<br><br>可以包含下列值中的 0 个、1 个或更多个：*电子邮件*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*<br><br> 可以使用 Graph API 添加/删除的值包括：*电子邮件*、*OfficeCommunicationsOnline*、*Yammer*<br>不可为 Null|
|状态|[domainState](domainstate.md)| 为域计划的异步操作的状态。 |

## <a name="relationships"></a>关系

通过导航属性公开目录中的域和其他对象之间的关系（如它们的验证记录和服务配置记录）。你可以通过在请求中定位这些导航属性来读取这些关系。

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) 集合| 只读，可为 NULL。|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md) 集合| Microsoft Online Services 可以使用域之前，客户添加到域 DNS 区域文件的 DNS 记录。<br>只读，可为 NULL。 |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md) 集合| 客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域 DNS 区域文件的 DNS 记录。<br>只读，可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 14,
  "passwordValidityPeriodInDays": 90,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
