---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关联的密钥凭据。 **应用程序和 servicePrincipal 实体的 keyCredentials** 属性是 **keyCredential 的集合**。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80583c40b61324b2b150c0ab377e4756f227ce39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135896"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="ba460-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba460-104">keyCredential resource type</span></span>

<span data-ttu-id="ba460-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba460-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba460-106">包含与应用程序关联的密钥凭据</span><span class="sxs-lookup"><span data-stu-id="ba460-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="ba460-107">.</span><span class="sxs-lookup"><span data-stu-id="ba460-107">.</span></span> <span data-ttu-id="ba460-108">**应用程序的 keyCredentials** [属性](application.md)</span><span class="sxs-lookup"><span data-stu-id="ba460-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="ba460-109">entity 是 **keyCredential 的集合**。</span><span class="sxs-lookup"><span data-stu-id="ba460-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="ba460-110">属性</span><span class="sxs-lookup"><span data-stu-id="ba460-110">Properties</span></span>
| <span data-ttu-id="ba460-111">属性</span><span class="sxs-lookup"><span data-stu-id="ba460-111">Property</span></span>     | <span data-ttu-id="ba460-112">类型</span><span class="sxs-lookup"><span data-stu-id="ba460-112">Type</span></span>   |<span data-ttu-id="ba460-113">说明</span><span class="sxs-lookup"><span data-stu-id="ba460-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba460-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba460-114">customKeyIdentifier</span></span>|<span data-ttu-id="ba460-115">Binary</span><span class="sxs-lookup"><span data-stu-id="ba460-115">Binary</span></span>| <span data-ttu-id="ba460-116">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="ba460-116">Custom key identifier</span></span> |
| <span data-ttu-id="ba460-117">displayName</span><span class="sxs-lookup"><span data-stu-id="ba460-117">displayName</span></span> | <span data-ttu-id="ba460-118">String</span><span class="sxs-lookup"><span data-stu-id="ba460-118">String</span></span> | <span data-ttu-id="ba460-119">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ba460-119">Friendly name for the key.</span></span> <span data-ttu-id="ba460-120">可选。</span><span class="sxs-lookup"><span data-stu-id="ba460-120">Optional.</span></span> |
|<span data-ttu-id="ba460-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ba460-121">endDateTime</span></span>|<span data-ttu-id="ba460-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba460-122">DateTimeOffset</span></span>|<span data-ttu-id="ba460-123">凭据过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ba460-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba460-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba460-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ba460-125">keyId</span><span class="sxs-lookup"><span data-stu-id="ba460-125">keyId</span></span>|<span data-ttu-id="ba460-126">Guid</span><span class="sxs-lookup"><span data-stu-id="ba460-126">Guid</span></span>|<span data-ttu-id="ba460-127">唯一标识符 (GUID) 的 GUID 值。</span><span class="sxs-lookup"><span data-stu-id="ba460-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="ba460-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba460-128">startDateTime</span></span>|<span data-ttu-id="ba460-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba460-129">DateTimeOffset</span></span>|<span data-ttu-id="ba460-130">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ba460-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba460-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba460-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ba460-132">type</span><span class="sxs-lookup"><span data-stu-id="ba460-132">type</span></span>|<span data-ttu-id="ba460-133">String</span><span class="sxs-lookup"><span data-stu-id="ba460-133">String</span></span>|<span data-ttu-id="ba460-134">密钥凭据的类型;例如，"Symmetric"。</span><span class="sxs-lookup"><span data-stu-id="ba460-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="ba460-135">usage</span><span class="sxs-lookup"><span data-stu-id="ba460-135">usage</span></span>|<span data-ttu-id="ba460-136">String</span><span class="sxs-lookup"><span data-stu-id="ba460-136">String</span></span>|<span data-ttu-id="ba460-137">一个描述可以使用密钥的目的的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="ba460-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="ba460-138">key</span><span class="sxs-lookup"><span data-stu-id="ba460-138">key</span></span>|<span data-ttu-id="ba460-139">二进制</span><span class="sxs-lookup"><span data-stu-id="ba460-139">Binary</span></span>| <span data-ttu-id="ba460-140">转换为 Base64 字符串的字节数组中的证书原始数据;例如 `[System.Convert]::ToBase64String($Cert.GetRawCertData())` ，。</span><span class="sxs-lookup"><span data-stu-id="ba460-140">The certificate's raw data in byte array converted to Base64 string; for example, `[System.Convert]::ToBase64String($Cert.GetRawCertData())`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba460-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba460-141">JSON representation</span></span>

<span data-ttu-id="ba460-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba460-142">Here is a JSON representation of the resource</span></span>

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

