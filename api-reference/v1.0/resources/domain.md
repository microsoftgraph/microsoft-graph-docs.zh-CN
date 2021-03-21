---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 62c48eca4f3672113c9eabbee7c420f7e2c9e4c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962460"
---
# <a name="domain-resource-type"></a>域资源类型

命名空间：microsoft.graph

表示与租户关联的域。

使用域操作将域与租户关联、验证域所有权并配置受支持的服务。  域操作使注册机构能够自动执行 Microsoft 365 等服务的域关联。 例如，作为域注册的一部分，注册机构可以启用电子邮件、网站、身份验证等的虚域。

将域与租户关联：

1. [将](../api/domain-post-domains.md) 域与租户关联。

2. [检索](../api/domain-list-verificationdnsrecords.md) 域验证记录。 使用域注册器或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。

3. [验证](../api/domain-verify.md) 域的所有权。 这将验证域，将 **isVerified** 属性设置为 `true` 。

4. [指示](../api/domain-update.md) 计划用于域的受支持服务。

5. [通过](../api/domain-list-serviceconfigurationrecords.md) 检索为域启用服务所需的记录列表来配置支持的服务。 使用域注册机构或 DNS 服务器配置将配置记录详细信息添加到域的区域文件。

## <a name="methods"></a>Methods

| 方法   | 返回类型 |说明|
|:---------------|:--------|:----------|
|[获取域](../api/domain-get.md) | [domain](domain.md) | 读取 domain 对象的属性和关系。|
|[创建域](../api/domain-post-domains.md) | [domain](domain.md) | 向租户添加域。 |
|[列出 domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) collection| 检索引用域的目录对象列表。|
|[列出 serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索域配置的域 DNS 记录列表。|
|[列出 verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索域 DNS 记录列表以用于域验证。|
|[更新域](../api/domain-update.md) | [domain](domain.md) |更新域。|
|[删除域](../api/domain-delete.md) | 无 |删除域。|
|[ForceDelete 域](../api/domain-forcedelete.md)|无|使用异步操作删除域。|
|[验证域](../api/domain-verify.md)|[domain](domain.md)|验证域的所有权。|

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|authenticationType|String| 指示域的已配置的身份验证类型。 值为 或 `Managed` `Federated` 。 `Managed` 指示 Azure AD 执行用户身份验证的云托管域。 `Federated` 指示通过 Active Directory 联合身份验证服务与标识提供程序（如租户本地 Active Directory）联合身份验证。 此属性是只读的，并且不可为 null。 |
|availabilityStatus|String| 此属性始终在使用 `null` verify 操作[](../api/domain-verify.md)时除外。 使用 [verify](../api/domain-verify.md) 操作 **时，响应** 中将返回一个域实体。 响应中 **domain** 实体的 **availabilityStatus** 属性是 `AvailableImmediately` 或 `EmailVerifiedDomainTakeoverScheduled` 。|
|id|String| 域的完全限定名称。 键、不可变、不可为 null、唯一。 |
|isAdminManaged|Boolean| 如果域的 DNS 记录管理已委派给 `false` Microsoft 365，则属性的值为 。 否则，值为 `true` 。 不可为 null |
|isDefault|Boolean| `true` 如果这是用于用户创建的默认域。 每个公司只有一个默认域。 不可为 null |
|isInitial|Boolean| `true` 如果这是由用户创建的初始Microsoft Online Services (companyname.onmicrosoft.com) 。 每个公司只有一个初始域。 不可为 null |
|isRoot|Boolean| `true` 如果域是已验证的根域。 否则 `false` ，如果域是子域或未经验证。 不可为 null |
|isVerified|Boolean| `true` 如果域已完成域所有权验证。 不可为 null |
|passwordNotificationWindowInDays|Int32|指定用户收到其密码将过期的通知前的天数。 如果未设置该属性，则使用默认值 14 天。|
|passwordValidityPeriodInDays|Int32| 指定密码在必须更改之前的有效时间长度。 如果未设置该属性，则使用默认值 90 天。 |
|supportedServices|String collection| 分配给域的功能。 可以包含 `0` 、 `1` 或更多以下值： `Email` 、 、 、 、 、 、 、 `Sharepoint` `EmailInternalRelayOnly` `OfficeCommunicationsOnline` `SharePointDefaultDomain` `FullRedelegation` `SharePointPublic` `OrgIdAuthentication` `Yammer` `Intune` 。 可以使用 Graph API 添加/删除的值包括 `Email` `OfficeCommunicationsOnline` ：、、。 `Yammer` 不可为 null|
|state|[domainState](domainstate.md)| 为域安排的异步操作的状态。 |

## <a name="relationships"></a>关系

域与目录中的其他对象（如其验证记录和服务配置记录）之间的关系通过导航属性公开。 可以通过在请求中定位这些导航属性来读取这些关系。

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) collection| 只读，可为空|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md) 集合| 在 Microsoft Online Services 使用域之前，客户添加到域的 DNS 区域文件的 DNS 记录。 只读，可为空 |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md) 集合| 客户添加到域的 DNS 区域文件的 DNS 记录，客户可以使用 Azure AD 完成域所有权验证。 只读，可为空|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

