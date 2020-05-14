---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体相关联的密钥凭据。 Application 和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 40837844b7ab78f86cd57438adeb08ceb97d52ad
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43441494"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="68cab-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="68cab-104">keyCredential resource type</span></span>

<span data-ttu-id="68cab-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68cab-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68cab-106">包含与应用程序关联的密钥凭据</span><span class="sxs-lookup"><span data-stu-id="68cab-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="68cab-107">.</span><span class="sxs-lookup"><span data-stu-id="68cab-107">.</span></span> <span data-ttu-id="68cab-108">[应用程序](application.md)的**keyCredentials**属性</span><span class="sxs-lookup"><span data-stu-id="68cab-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="68cab-109">实体是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="68cab-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="68cab-110">属性</span><span class="sxs-lookup"><span data-stu-id="68cab-110">Properties</span></span>
| <span data-ttu-id="68cab-111">属性</span><span class="sxs-lookup"><span data-stu-id="68cab-111">Property</span></span>     | <span data-ttu-id="68cab-112">类型</span><span class="sxs-lookup"><span data-stu-id="68cab-112">Type</span></span>   |<span data-ttu-id="68cab-113">说明</span><span class="sxs-lookup"><span data-stu-id="68cab-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68cab-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="68cab-114">customKeyIdentifier</span></span>|<span data-ttu-id="68cab-115">Binary</span><span class="sxs-lookup"><span data-stu-id="68cab-115">Binary</span></span>| <span data-ttu-id="68cab-116">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="68cab-116">Custom key identifier</span></span> |
| <span data-ttu-id="68cab-117">displayName</span><span class="sxs-lookup"><span data-stu-id="68cab-117">displayName</span></span> | <span data-ttu-id="68cab-118">String</span><span class="sxs-lookup"><span data-stu-id="68cab-118">String</span></span> | <span data-ttu-id="68cab-119">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="68cab-119">Friendly name for the key.</span></span> <span data-ttu-id="68cab-120">可选。</span><span class="sxs-lookup"><span data-stu-id="68cab-120">Optional.</span></span> |
|<span data-ttu-id="68cab-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="68cab-121">endDateTime</span></span>|<span data-ttu-id="68cab-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68cab-122">DateTimeOffset</span></span>|<span data-ttu-id="68cab-123">凭据到期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="68cab-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68cab-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="68cab-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="68cab-125">keyId</span><span class="sxs-lookup"><span data-stu-id="68cab-125">keyId</span></span>|<span data-ttu-id="68cab-126">Guid</span><span class="sxs-lookup"><span data-stu-id="68cab-126">Guid</span></span>|<span data-ttu-id="68cab-127">键的唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="68cab-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="68cab-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="68cab-128">startDateTime</span></span>|<span data-ttu-id="68cab-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68cab-129">DateTimeOffset</span></span>|<span data-ttu-id="68cab-130">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="68cab-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68cab-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="68cab-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="68cab-132">type</span><span class="sxs-lookup"><span data-stu-id="68cab-132">type</span></span>|<span data-ttu-id="68cab-133">String</span><span class="sxs-lookup"><span data-stu-id="68cab-133">String</span></span>|<span data-ttu-id="68cab-134">密钥凭据的类型;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="68cab-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="68cab-135">使用率</span><span class="sxs-lookup"><span data-stu-id="68cab-135">usage</span></span>|<span data-ttu-id="68cab-136">String</span><span class="sxs-lookup"><span data-stu-id="68cab-136">String</span></span>|<span data-ttu-id="68cab-137">一个描述可对其使用密钥的用途的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="68cab-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="68cab-138">key</span><span class="sxs-lookup"><span data-stu-id="68cab-138">key</span></span>|<span data-ttu-id="68cab-139">二进制</span><span class="sxs-lookup"><span data-stu-id="68cab-139">Binary</span></span>| <span data-ttu-id="68cab-140">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="68cab-140">Value for the key credential.</span></span> <span data-ttu-id="68cab-141">应为 base 64 编码值。</span><span class="sxs-lookup"><span data-stu-id="68cab-141">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68cab-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68cab-142">JSON representation</span></span>

<span data-ttu-id="68cab-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68cab-143">Here is a JSON representation of the resource</span></span>

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
