---
title: teamworkUserIdentity 资源类型
description: 表示用户Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0c50856a2b7051a631cd14ab3985cd8724bfe4c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211306"
---
# <a name="teamworkuseridentity-resource-type"></a><span data-ttu-id="68ad0-103">teamworkUserIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="68ad0-103">teamworkUserIdentity resource type</span></span>

<span data-ttu-id="68ad0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68ad0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68ad0-105">表示 **用户Microsoft Teams。**</span><span class="sxs-lookup"><span data-stu-id="68ad0-105">Represents a **user** in Microsoft Teams.</span></span>


<span data-ttu-id="68ad0-106">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="68ad0-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="68ad0-107">属性</span><span class="sxs-lookup"><span data-stu-id="68ad0-107">Properties</span></span>
|<span data-ttu-id="68ad0-108">属性</span><span class="sxs-lookup"><span data-stu-id="68ad0-108">Property</span></span>|<span data-ttu-id="68ad0-109">类型</span><span class="sxs-lookup"><span data-stu-id="68ad0-109">Type</span></span>|<span data-ttu-id="68ad0-110">说明</span><span class="sxs-lookup"><span data-stu-id="68ad0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68ad0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="68ad0-111">displayName</span></span>|<span data-ttu-id="68ad0-112">String</span><span class="sxs-lookup"><span data-stu-id="68ad0-112">String</span></span>|<span data-ttu-id="68ad0-113">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="68ad0-113">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="68ad0-114">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="68ad0-114">Display name of the user.</span></span> <span data-ttu-id="68ad0-115">可选。</span><span class="sxs-lookup"><span data-stu-id="68ad0-115">Optional.</span></span>|
|<span data-ttu-id="68ad0-116">id</span><span class="sxs-lookup"><span data-stu-id="68ad0-116">id</span></span>|<span data-ttu-id="68ad0-117">String</span><span class="sxs-lookup"><span data-stu-id="68ad0-117">String</span></span>|<span data-ttu-id="68ad0-118">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="68ad0-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="68ad0-119">用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="68ad0-119">ID of the user.</span></span> |
|<span data-ttu-id="68ad0-120">userIdentityType</span><span class="sxs-lookup"><span data-stu-id="68ad0-120">userIdentityType</span></span>|<span data-ttu-id="68ad0-121">teamworkUserIdentityType</span><span class="sxs-lookup"><span data-stu-id="68ad0-121">teamworkUserIdentityType</span></span>| <span data-ttu-id="68ad0-122">用户类型。</span><span class="sxs-lookup"><span data-stu-id="68ad0-122">Type of user.</span></span> <span data-ttu-id="68ad0-123">可能的值是 `aadUser` `onPremiseAadUser` `anonymousGuest` ：、、、、、、 `federatedUser` `personalMicrosoftAccountUser` 和 `skypeUser` `phoneUser` 。</span><span class="sxs-lookup"><span data-stu-id="68ad0-123">Possible values are: `aadUser`, `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, and `phoneUser`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68ad0-124">关系</span><span class="sxs-lookup"><span data-stu-id="68ad0-124">Relationships</span></span>
<span data-ttu-id="68ad0-125">无。</span><span class="sxs-lookup"><span data-stu-id="68ad0-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68ad0-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68ad0-126">JSON representation</span></span>
<span data-ttu-id="68ad0-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68ad0-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

