---
title: teamworkApplicationIdentity 资源类型
description: 表示应用程序中Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b7e6c17b70e7f30e102e270d2d98b406e01dcae3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211275"
---
# <a name="teamworkapplicationidentity-resource-type"></a><span data-ttu-id="9d69a-103">teamworkApplicationIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d69a-103">teamworkApplicationIdentity resource type</span></span>

<span data-ttu-id="9d69a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d69a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d69a-105">表示 **应用程序中** Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="9d69a-105">Represents an **application** in Microsoft Teams.</span></span> <span data-ttu-id="9d69a-106">`teamworkApplicationIdentity` 用于表示消息中的自动程序@mentioned传出 webhook。</span><span class="sxs-lookup"><span data-stu-id="9d69a-106">`teamworkApplicationIdentity` is used to represent bots and outgoing webhooks @mentioned in messages.</span></span>


<span data-ttu-id="9d69a-107">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="9d69a-107">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9d69a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d69a-108">Properties</span></span>
|<span data-ttu-id="9d69a-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d69a-109">Property</span></span>|<span data-ttu-id="9d69a-110">类型</span><span class="sxs-lookup"><span data-stu-id="9d69a-110">Type</span></span>|<span data-ttu-id="9d69a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d69a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d69a-112">applicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="9d69a-112">applicationIdentityType</span></span>|<span data-ttu-id="9d69a-113">teamworkApplicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="9d69a-113">teamworkApplicationIdentityType</span></span>| <span data-ttu-id="9d69a-114">引用的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="9d69a-114">Type of application that is referenced.</span></span> <span data-ttu-id="9d69a-115">可能的值是 `aadApplication` `bot` `tenantBot` ：、、、 `office365Connector` 和 `outgoingWebhook` 。</span><span class="sxs-lookup"><span data-stu-id="9d69a-115">Possible values are: `aadApplication`, `bot`, `tenantBot`, `office365Connector`, and `outgoingWebhook`.</span></span>|
|<span data-ttu-id="9d69a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9d69a-116">displayName</span></span>|<span data-ttu-id="9d69a-117">String</span><span class="sxs-lookup"><span data-stu-id="9d69a-117">String</span></span>|<span data-ttu-id="9d69a-118">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="9d69a-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="9d69a-119">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d69a-119">Display name of the application.</span></span> <span data-ttu-id="9d69a-120">可选。</span><span class="sxs-lookup"><span data-stu-id="9d69a-120">Optional.</span></span>|
|<span data-ttu-id="9d69a-121">id</span><span class="sxs-lookup"><span data-stu-id="9d69a-121">id</span></span>|<span data-ttu-id="9d69a-122">String</span><span class="sxs-lookup"><span data-stu-id="9d69a-122">String</span></span>|<span data-ttu-id="9d69a-123">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="9d69a-123">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="9d69a-124">应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="9d69a-124">ID of the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d69a-125">关系</span><span class="sxs-lookup"><span data-stu-id="9d69a-125">Relationships</span></span>
<span data-ttu-id="9d69a-126">无。</span><span class="sxs-lookup"><span data-stu-id="9d69a-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d69a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d69a-127">JSON representation</span></span>
<span data-ttu-id="9d69a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d69a-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

