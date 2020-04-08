---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cd1cc0e199848243fd9957f0741f609e052af6e6
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178938"
---
# <a name="domain-resource-type"></a>域资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与租户关联的域。

使用域操作将域与租户相关联，验证域所有权并配置受支持的服务。  域操作使注册机构能够自动为 Office 365 等服务的域关联。 例如，在注册域的过程中，注册机构可以为电子邮件、网站、身份验证等启用虚域。

将域与租户相关联：

1. 将域与租户[相关联](../api/domain-post-domains.md)。

2. [检索](../api/domain-list-verificationdnsrecords.md)域验证记录。 使用域注册机构或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。

3. [验证](../api/domain-verify.md)域的所有权。 这将验证域并将*isVerified*属性设置为*true*。

4. [指明](../api/domain-update.md)计划与域一起使用的受支持服务。

5. 通过检索为域启用服务所需的记录列表来[配置](../api/domain-list-serviceconfigurationrecords.md)受支持的服务。 使用域注册机构或 DNS 服务器配置将配置记录详细信息添加到域的区域文件中。

## <a name="methods"></a>方法

| 方法   | 返回类型 |说明|
|:---------------|:--------|:----------|
|[获取域](../api/domain-get.md) | [domain](domain.md) | 读取域对象的属性和关系。|
|[创建域](../api/domain-post-domains.md) | [domain](domain.md) | 向租户添加域。 |
|[列出 domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) collection| 使用对域的引用检索目录对象的列表。|
|[列出 serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md)集合|  检索域配置的域 DNS 记录列表。|
|[列出 verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md)集合|  检索域验证的域 DNS 记录列表。|
|[更新域](../api/domain-update.md) | [domain](domain.md) |更新域。|
|[删除域](../api/domain-delete.md) | 无 |删除域。|
|[ForceDelete 域](../api/domain-forcedelete.md)|无|使用异步操作删除域。|
|[验证域](../api/domain-verify.md)|[domain](domain.md)|验证域的所有权。|

## <a name="properties"></a>属性

| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|authenticationType|String| 指示为域配置的身份验证类型。 值为 "*托管*" 或 "*联合*"。<br> *托管*表示 Azure AD 执行用户身份验证的云托管域。<br>*联合*指示身份验证通过使用标识提供程序（如通过 Active Directory 联合身份验证服务的租户的本地 Active directory）进行联合。 此属性为只读，且不可为 null。 |
|availabilityStatus|String| 除非使用了[verify](../api/domain-verify.md)操作，否则此属性始终为 null。 使用[验证](../api/domain-verify.md)操作时，会在响应中返回**域**实体。 响应中的**域**实体的**AvailabilityStatus**属性为*AvailableImmediately*或*EmailVerifiedDomainTakeoverScheduled*。|
|id|String| 域的完全限定的名称。 键、不可变、不可为 null、唯一 |
|isAdminManaged|布尔值| 如果域的 DNS 记录管理已委派给 Office 365，则该属性的值为 false。 否则，该值为 true。 不可为 null |
|isDefault|布尔值| 如果这是用于创建用户的默认域，则为 True。 每个公司只有一个默认域。 不可为 null |
|isInitial|Boolean| 如果这是 Microsoft Online Services （companyname.onmicrosoft.com）创建的初始域，则为 True。 每个公司只有一个初始域。 不可为 null |
|isRoot|布尔值| 如果域是经过验证的根域，则为 True。 否则，如果域是子域或未验证，则为 false。 不可为 null |
|isVerified|布尔值| 如果域已完成域所有权验证，则为 True。 不可为 null |
|passwordNotificationWindowInDays|Int32|指定用户收到其密码将到期的通知之前的天数。 如果未设置该属性，则将使用默认值14天。|
|passwordValidityPeriodInDays|Int32| 指定密码在必须更改之前有效的时间长度。 如果未设置该属性，则将使用默认值90天。 |
|supportedServices|String 集合| 分配给域的功能。<br><br>可以包含0个、1个或更多的以下值： *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*<br><br> 您可以使用 Graph API 添加/删除的值包括： *Email*、 *OfficeCommunicationsOnline*、 *Yammer*<br>不可为 null|
|state|[domainState](domainstate.md)| 为域计划的异步操作的状态。 |

## <a name="relationships"></a>关系

域和目录中的其他对象（如其验证记录和服务配置记录）之间的关系通过导航属性公开。 您可以通过在请求中将这些导航属性作为目标来读取这些关系。

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) collection| 只读、可以为 Null|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md)集合| 在 Microsoft Online services 可以使用域之前，客户添加到域的 DNS 区域文件中的 DNS 记录。<br>只读、可以为 Null |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md)集合| 在客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域的 DNS 区域文件中的 DNS 记录。<br>只读、可以为 Null|

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
