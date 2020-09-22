---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体相关联的密钥凭据。 Application 和 servicePrincipal 实体的 **keyCredentials** 属性是 **keyCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6c005a44827640ed7a61e61f07837a98021d9a9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078338"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="d3d8c-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3d8c-104">keyCredential resource type</span></span>

<span data-ttu-id="d3d8c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3d8c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d8c-106">包含与应用程序或服务主体相关联的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="d3d8c-107">[Application](application.md)和[ServicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="d3d8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3d8c-108">Properties</span></span>
| <span data-ttu-id="d3d8c-109">属性</span><span class="sxs-lookup"><span data-stu-id="d3d8c-109">Property</span></span>     | <span data-ttu-id="d3d8c-110">类型</span><span class="sxs-lookup"><span data-stu-id="d3d8c-110">Type</span></span>   |<span data-ttu-id="d3d8c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3d8c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3d8c-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="d3d8c-112">customKeyIdentifier</span></span>|<span data-ttu-id="d3d8c-113">Binary</span><span class="sxs-lookup"><span data-stu-id="d3d8c-113">Binary</span></span>| <span data-ttu-id="d3d8c-114">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="d3d8c-114">Custom key identifier</span></span> |
| <span data-ttu-id="d3d8c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d3d8c-115">displayName</span></span> | <span data-ttu-id="d3d8c-116">String</span><span class="sxs-lookup"><span data-stu-id="d3d8c-116">String</span></span> | <span data-ttu-id="d3d8c-117">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-117">Friendly name for the key.</span></span> <span data-ttu-id="d3d8c-118">可选。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-118">Optional.</span></span> |
|<span data-ttu-id="d3d8c-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d3d8c-119">endDateTime</span></span>|<span data-ttu-id="d3d8c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d8c-120">DateTimeOffset</span></span>|<span data-ttu-id="d3d8c-121">凭据到期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3d8c-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d3d8c-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d3d8c-123">keyId</span><span class="sxs-lookup"><span data-stu-id="d3d8c-123">keyId</span></span>|<span data-ttu-id="d3d8c-124">Guid</span><span class="sxs-lookup"><span data-stu-id="d3d8c-124">Guid</span></span>|<span data-ttu-id="d3d8c-125">密钥的唯一标识符 (GUID) 。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="d3d8c-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d3d8c-126">startDateTime</span></span>|<span data-ttu-id="d3d8c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d8c-127">DateTimeOffset</span></span>|<span data-ttu-id="d3d8c-128">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3d8c-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d3d8c-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d3d8c-130">type</span><span class="sxs-lookup"><span data-stu-id="d3d8c-130">type</span></span>|<span data-ttu-id="d3d8c-131">String</span><span class="sxs-lookup"><span data-stu-id="d3d8c-131">String</span></span>|<span data-ttu-id="d3d8c-132">密钥凭据的类型;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="d3d8c-133">使用率</span><span class="sxs-lookup"><span data-stu-id="d3d8c-133">usage</span></span>|<span data-ttu-id="d3d8c-134">String</span><span class="sxs-lookup"><span data-stu-id="d3d8c-134">String</span></span>|<span data-ttu-id="d3d8c-135">一个描述可对其使用密钥的用途的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="d3d8c-136">key</span><span class="sxs-lookup"><span data-stu-id="d3d8c-136">key</span></span>|<span data-ttu-id="d3d8c-137">二进制</span><span class="sxs-lookup"><span data-stu-id="d3d8c-137">Binary</span></span>| <span data-ttu-id="d3d8c-138">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-138">Value for the key credential.</span></span> <span data-ttu-id="d3d8c-139">应为 base 64 编码值。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3d8c-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3d8c-140">JSON representation</span></span>

<span data-ttu-id="d3d8c-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3d8c-141">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


