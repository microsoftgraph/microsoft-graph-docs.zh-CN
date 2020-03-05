---
title: userIdentity 资源类型
description: 在 Azure AD 审核日志的上下文中，这表示已启动或受审核活动影响的用户信息。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 304d5a27714d7e6e02183b372814c8cb16c4e0b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446791"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="0903b-103">userIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="0903b-103">userIdentity resource type</span></span>

<span data-ttu-id="0903b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0903b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0903b-105">在 Azure AD 审核日志的上下文中，这表示已启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="0903b-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="0903b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0903b-106">Properties</span></span>

| <span data-ttu-id="0903b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0903b-107">Property</span></span>     | <span data-ttu-id="0903b-108">类型</span><span class="sxs-lookup"><span data-stu-id="0903b-108">Type</span></span>   |<span data-ttu-id="0903b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0903b-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0903b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0903b-110">displayName</span></span> | <span data-ttu-id="0903b-111">String</span><span class="sxs-lookup"><span data-stu-id="0903b-111">String</span></span> | <span data-ttu-id="0903b-112">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0903b-112">The identity's display name.</span></span> <span data-ttu-id="0903b-113">请注意，这可能并不总是可用，也不是最新的。</span><span class="sxs-lookup"><span data-stu-id="0903b-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="0903b-114">id</span><span class="sxs-lookup"><span data-stu-id="0903b-114">id</span></span>          | <span data-ttu-id="0903b-115">String</span><span class="sxs-lookup"><span data-stu-id="0903b-115">String</span></span> | <span data-ttu-id="0903b-116">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0903b-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="0903b-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0903b-117">ipAddress</span></span>   | <span data-ttu-id="0903b-118">String</span><span class="sxs-lookup"><span data-stu-id="0903b-118">String</span></span>| <span data-ttu-id="0903b-119">指示执行活动的用户使用的客户端 IP 地址（仅限审核日志）。</span><span class="sxs-lookup"><span data-stu-id="0903b-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="0903b-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0903b-120">userPrincipalName</span></span> | <span data-ttu-id="0903b-121">字符串</span><span class="sxs-lookup"><span data-stu-id="0903b-121">String</span></span>  | <span data-ttu-id="0903b-122">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="0903b-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="0903b-123">**注意：** 在某些情况下，唯一标识符可能不可用。</span><span class="sxs-lookup"><span data-stu-id="0903b-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="0903b-124">在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="0903b-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0903b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0903b-125">JSON representation</span></span>

<span data-ttu-id="0903b-126">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0903b-126">Here is a JSON representation of the type.</span></span>

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
