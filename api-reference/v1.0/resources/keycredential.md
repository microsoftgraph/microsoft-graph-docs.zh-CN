---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关联的密钥凭据。 application 和 servicePrincipal 实体的 **keyCredentials** 属性是 **keyCredential 的集合**。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 05b0aa71059bcf0ef974e49fb012a3815386b9be
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722235"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="87e56-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="87e56-104">keyCredential resource type</span></span>

<span data-ttu-id="87e56-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87e56-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87e56-106">包含与应用程序关联的密钥凭据</span><span class="sxs-lookup"><span data-stu-id="87e56-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="87e56-107">.</span><span class="sxs-lookup"><span data-stu-id="87e56-107">.</span></span> <span data-ttu-id="87e56-108">**应用程序的 keyCredentials** [属性](application.md)</span><span class="sxs-lookup"><span data-stu-id="87e56-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="87e56-109">entity 是 **keyCredential 的集合**。</span><span class="sxs-lookup"><span data-stu-id="87e56-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="87e56-110">属性</span><span class="sxs-lookup"><span data-stu-id="87e56-110">Properties</span></span>
| <span data-ttu-id="87e56-111">属性</span><span class="sxs-lookup"><span data-stu-id="87e56-111">Property</span></span>     | <span data-ttu-id="87e56-112">类型</span><span class="sxs-lookup"><span data-stu-id="87e56-112">Type</span></span>   |<span data-ttu-id="87e56-113">说明</span><span class="sxs-lookup"><span data-stu-id="87e56-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87e56-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="87e56-114">customKeyIdentifier</span></span>|<span data-ttu-id="87e56-115">Binary</span><span class="sxs-lookup"><span data-stu-id="87e56-115">Binary</span></span>| <span data-ttu-id="87e56-116">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="87e56-116">Custom key identifier</span></span> |
| <span data-ttu-id="87e56-117">displayName</span><span class="sxs-lookup"><span data-stu-id="87e56-117">displayName</span></span> | <span data-ttu-id="87e56-118">字符串</span><span class="sxs-lookup"><span data-stu-id="87e56-118">String</span></span> | <span data-ttu-id="87e56-119">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="87e56-119">Friendly name for the key.</span></span> <span data-ttu-id="87e56-120">可选。</span><span class="sxs-lookup"><span data-stu-id="87e56-120">Optional.</span></span> |
|<span data-ttu-id="87e56-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87e56-121">endDateTime</span></span>|<span data-ttu-id="87e56-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e56-122">DateTimeOffset</span></span>|<span data-ttu-id="87e56-123">凭据过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="87e56-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87e56-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="87e56-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="87e56-125">keyId</span><span class="sxs-lookup"><span data-stu-id="87e56-125">keyId</span></span>|<span data-ttu-id="87e56-126">Guid</span><span class="sxs-lookup"><span data-stu-id="87e56-126">Guid</span></span>|<span data-ttu-id="87e56-127">该密钥 (GUID) 标识符。</span><span class="sxs-lookup"><span data-stu-id="87e56-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="87e56-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87e56-128">startDateTime</span></span>|<span data-ttu-id="87e56-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e56-129">DateTimeOffset</span></span>|<span data-ttu-id="87e56-130">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="87e56-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87e56-131">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="87e56-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="87e56-132">type</span><span class="sxs-lookup"><span data-stu-id="87e56-132">type</span></span>|<span data-ttu-id="87e56-133">字符串</span><span class="sxs-lookup"><span data-stu-id="87e56-133">String</span></span>|<span data-ttu-id="87e56-134">密钥凭据的类型;例如，"Symmetric"。</span><span class="sxs-lookup"><span data-stu-id="87e56-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="87e56-135">usage</span><span class="sxs-lookup"><span data-stu-id="87e56-135">usage</span></span>|<span data-ttu-id="87e56-136">字符串</span><span class="sxs-lookup"><span data-stu-id="87e56-136">String</span></span>|<span data-ttu-id="87e56-137">一个描述密钥的用途的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="87e56-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="87e56-138">key</span><span class="sxs-lookup"><span data-stu-id="87e56-138">key</span></span>|<span data-ttu-id="87e56-139">二进制</span><span class="sxs-lookup"><span data-stu-id="87e56-139">Binary</span></span>| <span data-ttu-id="87e56-140">转换为 Base64 字符串的字节数组中的证书原始数据;例如， `[System.Convert]::ToBase64String($Cert.GetRawCertData())` 。</span><span class="sxs-lookup"><span data-stu-id="87e56-140">The certificate's raw data in byte array converted to Base64 string; for example, `[System.Convert]::ToBase64String($Cert.GetRawCertData())`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87e56-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87e56-141">JSON representation</span></span>

<span data-ttu-id="87e56-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87e56-142">Here is a JSON representation of the resource</span></span>

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

