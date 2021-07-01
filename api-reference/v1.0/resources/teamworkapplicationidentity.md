---
title: teamworkApplicationIdentity 资源类型
description: 表示应用程序中Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 67e1ed4365febae44032c09d94656d2e3ac0b504
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211082"
---
# <a name="teamworkapplicationidentity-resource-type"></a><span data-ttu-id="bef36-103">teamworkApplicationIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="bef36-103">teamworkApplicationIdentity resource type</span></span>

<span data-ttu-id="bef36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bef36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bef36-105">表示 **应用程序中** Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="bef36-105">Represents an **application** in Microsoft Teams.</span></span> <span data-ttu-id="bef36-106">`teamworkApplicationIdentity` 用于表示消息中的自动程序@mentioned传出 webhook。</span><span class="sxs-lookup"><span data-stu-id="bef36-106">`teamworkApplicationIdentity` is used to represent bots and outgoing webhooks @mentioned in messages.</span></span>


<span data-ttu-id="bef36-107">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="bef36-107">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bef36-108">属性</span><span class="sxs-lookup"><span data-stu-id="bef36-108">Properties</span></span>
|<span data-ttu-id="bef36-109">属性</span><span class="sxs-lookup"><span data-stu-id="bef36-109">Property</span></span>|<span data-ttu-id="bef36-110">类型</span><span class="sxs-lookup"><span data-stu-id="bef36-110">Type</span></span>|<span data-ttu-id="bef36-111">说明</span><span class="sxs-lookup"><span data-stu-id="bef36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef36-112">applicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="bef36-112">applicationIdentityType</span></span>|<span data-ttu-id="bef36-113">teamworkApplicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="bef36-113">teamworkApplicationIdentityType</span></span>| <span data-ttu-id="bef36-114">引用的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="bef36-114">Type of application that is referenced.</span></span> <span data-ttu-id="bef36-115">可能的值是 `aadApplication` `bot` `tenantBot` ：、、、、 `office365Connector` `outgoingWebhook` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="bef36-115">Possible values are: `aadApplication`, `bot`, `tenantBot`, `office365Connector`, `outgoingWebhook`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bef36-116">displayName</span><span class="sxs-lookup"><span data-stu-id="bef36-116">displayName</span></span>|<span data-ttu-id="bef36-117">String</span><span class="sxs-lookup"><span data-stu-id="bef36-117">String</span></span>|<span data-ttu-id="bef36-118">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="bef36-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="bef36-119">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bef36-119">Display name of the application.</span></span> <span data-ttu-id="bef36-120">可选。</span><span class="sxs-lookup"><span data-stu-id="bef36-120">Optional.</span></span>|
|<span data-ttu-id="bef36-121">id</span><span class="sxs-lookup"><span data-stu-id="bef36-121">id</span></span>|<span data-ttu-id="bef36-122">String</span><span class="sxs-lookup"><span data-stu-id="bef36-122">String</span></span>|<span data-ttu-id="bef36-123">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="bef36-123">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="bef36-124">应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="bef36-124">ID of the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bef36-125">关系</span><span class="sxs-lookup"><span data-stu-id="bef36-125">Relationships</span></span>
<span data-ttu-id="bef36-126">无。</span><span class="sxs-lookup"><span data-stu-id="bef36-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bef36-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bef36-127">JSON representation</span></span>
<span data-ttu-id="bef36-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bef36-128">The following is a JSON representation of the resource.</span></span>
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

