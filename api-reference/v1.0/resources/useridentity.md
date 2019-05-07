---
title: userIdentity 资源类型
description: 在 Azure AD 审核日志的上下文中, 这表示已启动或受审核活动影响的用户信息。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 018bc8ca3713822295d0acef66e8ec075d276cfe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629227"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="5ac67-103">userIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ac67-103">userIdentity resource type</span></span>

<span data-ttu-id="5ac67-104">在 Azure AD 审核日志的上下文中, 这表示已启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="5ac67-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="5ac67-105">属性</span><span class="sxs-lookup"><span data-stu-id="5ac67-105">Properties</span></span>

| <span data-ttu-id="5ac67-106">属性</span><span class="sxs-lookup"><span data-stu-id="5ac67-106">Property</span></span>     | <span data-ttu-id="5ac67-107">类型</span><span class="sxs-lookup"><span data-stu-id="5ac67-107">Type</span></span>   |<span data-ttu-id="5ac67-108">说明</span><span class="sxs-lookup"><span data-stu-id="5ac67-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ac67-109">displayName</span><span class="sxs-lookup"><span data-stu-id="5ac67-109">displayName</span></span> | <span data-ttu-id="5ac67-110">String</span><span class="sxs-lookup"><span data-stu-id="5ac67-110">String</span></span> | <span data-ttu-id="5ac67-111">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5ac67-111">The identity's display name.</span></span> <span data-ttu-id="5ac67-112">请注意, 这可能并不总是可用, 也不是最新的。</span><span class="sxs-lookup"><span data-stu-id="5ac67-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="5ac67-113">id</span><span class="sxs-lookup"><span data-stu-id="5ac67-113">id</span></span>          | <span data-ttu-id="5ac67-114">String</span><span class="sxs-lookup"><span data-stu-id="5ac67-114">String</span></span> | <span data-ttu-id="5ac67-115">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ac67-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="5ac67-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5ac67-116">ipAddress</span></span>   | <span data-ttu-id="5ac67-117">String</span><span class="sxs-lookup"><span data-stu-id="5ac67-117">String</span></span>| <span data-ttu-id="5ac67-118">指示执行活动的用户使用的客户端 IP 地址 (仅限审核日志)。</span><span class="sxs-lookup"><span data-stu-id="5ac67-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="5ac67-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ac67-119">userPrincipalName</span></span> | <span data-ttu-id="5ac67-120">字符串</span><span class="sxs-lookup"><span data-stu-id="5ac67-120">String</span></span>  | <span data-ttu-id="5ac67-121">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="5ac67-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="5ac67-122">**注意:** 在某些情况下, 唯一标识符可能不可用。</span><span class="sxs-lookup"><span data-stu-id="5ac67-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="5ac67-123">在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="5ac67-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ac67-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ac67-124">JSON representation</span></span>

<span data-ttu-id="5ac67-125">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ac67-125">Here is a JSON representation of the type.</span></span>

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
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
