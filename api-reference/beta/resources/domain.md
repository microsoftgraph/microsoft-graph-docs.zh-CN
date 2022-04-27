---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 981b64bf5becec9bc51072700580781f855815bf
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060561"
---
# <a name="domain-resource-type"></a>域资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与租户关联的域。

使用域操作将域关联到租户，验证域所有权并配置受支持的服务。  域操作使注册机构能够为服务（如Microsoft 365）自动关联域关联。 例如，作为域注册的一部分，注册机构可以为电子邮件、网站、身份验证等启用虚荣域。

若要将域与租户关联，请执行下表操作：

1. [将](../api/domain-post-domains.md) 域与租户关联。

2. [检索](../api/domain-list-verificationdnsrecords.md) 域验证记录。 使用域注册机构或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。

3. [验证](../api/domain-verify.md) 域的所有权。 这将验证域并将 **isVerified** 属性设置为 `true`。

4. [指示](../api/domain-update.md) 计划与域一起使用的受支持服务。

5. 通过检索启用域服务所需的记录列表来[配置](../api/domain-list-serviceconfigurationrecords.md)支持的服务。 使用域注册机构或 DNS 服务器配置将配置记录详细信息添加到域的区域文件。

## <a name="methods"></a>方法

| 方法   | 返回类型 |说明|
|:---------------|:--------|:----------|
|[获取域](../api/domain-get.md) | [domain](domain.md) | 读取域对象的属性和关系。|
|[创建域](../api/domain-post-domains.md) | [domain](domain.md) | 向租户添加域。 |
|[列出域](../api/domain-list.md) | [domain](domain.md) | 检索链接到租户的所有域。 |
|[列出 domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) collection| 检索引用域的目录对象列表。|
|[列出 serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索域配置的域 DNS 记录列表。|
|[列出 verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md) 集合|  检索域 DNS 记录的列表以进行域验证。|
|[更新域](../api/domain-update.md) | [domain](domain.md) |更新域。|
|[删除域](../api/domain-delete.md) | 无 |删除域。|
|[ForceDelete 域](../api/domain-forcedelete.md)|无|使用异步操作删除域。|
|[验证域](../api/domain-verify.md)|[domain](domain.md)|验证域的所有权。|

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|authenticationType|String| 指示为域配置的身份验证类型。 值为或 `Managed` `Federated`. `Managed`指示Azure AD执行用户身份验证的云托管域。 `Federated`指示身份验证通过Active Directory 联合身份验证服务与标识提供者（例如租户的本地 Active Directory）联合。 此属性为只读属性，不可为 null。 |
|availabilityStatus|String| 此属性始终 `null` 是使用 [验证](../api/domain-verify.md) 操作时除外。 使用 [验证](../api/domain-verify.md) 操作时，会在响应中返回 **域** 实体。 响应中 **域** 实体的 **availabilityStatus** 属性为或 `AvailableImmediately` `EmailVerifiedDomainTakeoverScheduled`。|
|id|String| 域的完全限定名称。 键，不可变，不可为 null，唯一。 |
|isAdminManaged|Boolean| 该属性的值是`false`域的 DNS 记录管理是否已委托给Microsoft 365。 否则，值为 `true`. 不可为 null |
|isDefault|Boolean| `true` 如果这是用于创建用户的默认域。 每个公司只有一个默认域。 不可为 null |
|isInitial|Boolean| `true` 如果这是 Microsoft Online Services (companyname.onmicrosoft.com) 创建的初始域。 每个公司只有一个初始域。 不可为 null |
|isRoot|Boolean| `true` 如果域是已验证的根域， 否则， `false` 如果域是子域或未验证。 不可为 null |
|isVerified|Boolean| `true` 如果域已完成域所有权验证。 不可为 null |
|passwordNotificationWindowInDays|Int32|指定用户收到其密码过期通知之前的天数。 如果未设置该属性，将使用默认值 14 天。|
|passwordValidityPeriodInDays|Int32| 指定必须更改密码之前密码有效的时间长度。 如果未设置该属性，将使用默认值 90 天。 |
|supportedServices|字符串集合| 分配给域的功能。 可以包括`0``1`或包含以下值的更多内容：`Email`、、`Sharepoint`、`SharePointDefaultDomain``OfficeCommunicationsOnline``EmailInternalRelayOnly`、、、`SharePointPublic``FullRedelegation`、、`OrgIdAuthentication`、。 `Intune``Yammer` 可以使用图形 API添加/删除的值包括： `Email`， ， `OfficeCommunicationsOnline`。 `Yammer` 不可为 null|
|state|[domainState](domainstate.md)| 为域计划异步操作的状态。 |

## <a name="relationships"></a>关系

域与目录中的其他对象（如验证记录和服务配置记录）之间的关系通过导航属性公开。 可以通过在请求中针对这些导航属性来读取这些关系。

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) collection| 只读，可为 Null|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md) 集合| 在 Microsoft Online 服务使用域之前，客户会将 DNS 记录添加到域的 DNS 区域文件中。 只读，可为 Null |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md) 集合| 在客户使用Azure AD完成域所有权验证之前，DNS 记录客户添加到域的 DNS 区域文件。 只读，可为 Null|
|federationConfiguration|[internalDomainFederation](../resources/internaldomainfederation.md)| 客户在与Azure AD联合时配置的域设置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "suppressions": []
}
-->


