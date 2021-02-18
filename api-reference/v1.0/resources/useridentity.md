---
title: userIdentity 资源类型
description: 在 Azure AD 审核日志中，这表示启动或受审核活动影响的用户信息。
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 814b7106bf738711099d6d6e8d5e821b7b638318
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292159"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="a255c-103">userIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="a255c-103">userIdentity resource type</span></span>

<span data-ttu-id="a255c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a255c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a255c-105">在 Azure AD 审核日志中，这表示启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="a255c-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="a255c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a255c-106">Properties</span></span>

| <span data-ttu-id="a255c-107">属性</span><span class="sxs-lookup"><span data-stu-id="a255c-107">Property</span></span>     | <span data-ttu-id="a255c-108">类型</span><span class="sxs-lookup"><span data-stu-id="a255c-108">Type</span></span>   |<span data-ttu-id="a255c-109">说明</span><span class="sxs-lookup"><span data-stu-id="a255c-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a255c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a255c-110">displayName</span></span> | <span data-ttu-id="a255c-111">String</span><span class="sxs-lookup"><span data-stu-id="a255c-111">String</span></span> | <span data-ttu-id="a255c-112">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a255c-112">The identity's display name.</span></span> <span data-ttu-id="a255c-113">请注意，这可能并不总是可用或最新的。</span><span class="sxs-lookup"><span data-stu-id="a255c-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="a255c-114">id</span><span class="sxs-lookup"><span data-stu-id="a255c-114">id</span></span>          | <span data-ttu-id="a255c-115">String</span><span class="sxs-lookup"><span data-stu-id="a255c-115">String</span></span> | <span data-ttu-id="a255c-116">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a255c-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="a255c-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="a255c-117">ipAddress</span></span>   | <span data-ttu-id="a255c-118">String</span><span class="sxs-lookup"><span data-stu-id="a255c-118">String</span></span>| <span data-ttu-id="a255c-119">指示仅与用户一起执行活动 (审核日志使用的) 。</span><span class="sxs-lookup"><span data-stu-id="a255c-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="a255c-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a255c-120">userPrincipalName</span></span> | <span data-ttu-id="a255c-121">String</span><span class="sxs-lookup"><span data-stu-id="a255c-121">String</span></span>  | <span data-ttu-id="a255c-122">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="a255c-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="a255c-123">**注意：** 在某些情况下，唯一标识符可能不可用。</span><span class="sxs-lookup"><span data-stu-id="a255c-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="a255c-124">在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="a255c-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a255c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a255c-125">JSON representation</span></span>

<span data-ttu-id="a255c-126">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a255c-126">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

