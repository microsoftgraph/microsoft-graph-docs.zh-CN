---
title: domainDnsTxtRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件的 TXT 记录。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f63b671135edceb715aa4b3641b4bf189b74a33
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761379"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="5e1ac-103">domainDnsTxtRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e1ac-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="5e1ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e1ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e1ac-105">表示添加到租户中特定域的 DNS 区域文件的 TXT 记录。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="5e1ac-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5e1ac-107">方法</span><span class="sxs-lookup"><span data-stu-id="5e1ac-107">Methods</span></span>
<span data-ttu-id="5e1ac-108">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="5e1ac-109">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5e1ac-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e1ac-110">Properties</span></span>
| <span data-ttu-id="5e1ac-111">属性</span><span class="sxs-lookup"><span data-stu-id="5e1ac-111">Property</span></span>     | <span data-ttu-id="5e1ac-112">类型</span><span class="sxs-lookup"><span data-stu-id="5e1ac-112">Type</span></span>   |<span data-ttu-id="5e1ac-113">说明</span><span class="sxs-lookup"><span data-stu-id="5e1ac-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1ac-114">id</span><span class="sxs-lookup"><span data-stu-id="5e1ac-114">id</span></span>|<span data-ttu-id="5e1ac-115">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1ac-115">String</span></span>| <span data-ttu-id="5e1ac-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="5e1ac-117">不可为空，只读。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="5e1ac-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="5e1ac-118">isOptional</span></span>|<span data-ttu-id="5e1ac-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e1ac-119">Boolean</span></span>| <span data-ttu-id="5e1ac-120">如果为 false，则客户必须在 DNS 主机上配置 TXT 记录，Microsoft Online Services该域正常运行。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="5e1ac-121">label</span><span class="sxs-lookup"><span data-stu-id="5e1ac-121">label</span></span>|<span data-ttu-id="5e1ac-122">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1ac-122">String</span></span>| <span data-ttu-id="5e1ac-123">在 DNS 主机上配置TXT 记录的名称属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="5e1ac-124">recordType</span><span class="sxs-lookup"><span data-stu-id="5e1ac-124">recordType</span></span>|<span data-ttu-id="5e1ac-125">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1ac-125">String</span></span>| <span data-ttu-id="5e1ac-126">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-126">Type of DNS record.</span></span> <span data-ttu-id="5e1ac-127">该值始终为 *Txt*。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-127">The value is always *Txt*.</span></span> <span data-ttu-id="5e1ac-128">键</span><span class="sxs-lookup"><span data-stu-id="5e1ac-128">Key</span></span> |
|<span data-ttu-id="5e1ac-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="5e1ac-129">supportedService</span></span>|<span data-ttu-id="5e1ac-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1ac-130">String</span></span>| <span data-ttu-id="5e1ac-131">依赖此 TXT 记录的 Microsoft Online Service 或功能。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="5e1ac-132">可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           </span><span class="sxs-lookup"><span data-stu-id="5e1ac-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="5e1ac-133">text</span><span class="sxs-lookup"><span data-stu-id="5e1ac-133">text</span></span>|<span data-ttu-id="5e1ac-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1ac-134">String</span></span>| <span data-ttu-id="5e1ac-135">在 DNS 主机上配置 *文本* 属性时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="5e1ac-136">ttl</span><span class="sxs-lookup"><span data-stu-id="5e1ac-136">ttl</span></span>|<span data-ttu-id="5e1ac-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5e1ac-137">Int32</span></span>| <span data-ttu-id="5e1ac-138">在 DNS 主机上配置 MX 记录的 ttl (*ttl*) 时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="5e1ac-139">不可为 null</span><span class="sxs-lookup"><span data-stu-id="5e1ac-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e1ac-140">关系</span><span class="sxs-lookup"><span data-stu-id="5e1ac-140">Relationships</span></span>
<span data-ttu-id="5e1ac-141">无</span><span class="sxs-lookup"><span data-stu-id="5e1ac-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e1ac-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e1ac-142">JSON representation</span></span>
<span data-ttu-id="5e1ac-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e1ac-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

