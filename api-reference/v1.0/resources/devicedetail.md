---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8730c6fefebadbd2c64937366c7b7de41537b11c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531673"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="17d86-104">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="17d86-104">deviceDetail resource type</span></span>

<span data-ttu-id="17d86-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17d86-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17d86-106">指示与用于登录的设备相关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="17d86-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="17d86-107">其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。</span><span class="sxs-lookup"><span data-stu-id="17d86-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="17d86-108">属性</span><span class="sxs-lookup"><span data-stu-id="17d86-108">Properties</span></span>

| <span data-ttu-id="17d86-109">属性</span><span class="sxs-lookup"><span data-stu-id="17d86-109">Property</span></span>     | <span data-ttu-id="17d86-110">类型</span><span class="sxs-lookup"><span data-stu-id="17d86-110">Type</span></span>   |<span data-ttu-id="17d86-111">说明</span><span class="sxs-lookup"><span data-stu-id="17d86-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17d86-112">浏览器</span><span class="sxs-lookup"><span data-stu-id="17d86-112">browser</span></span>|<span data-ttu-id="17d86-113">字符串</span><span class="sxs-lookup"><span data-stu-id="17d86-113">String</span></span>|<span data-ttu-id="17d86-114">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="17d86-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="17d86-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="17d86-115">deviceId</span></span>|<span data-ttu-id="17d86-116">String</span><span class="sxs-lookup"><span data-stu-id="17d86-116">String</span></span>|<span data-ttu-id="17d86-117">指用于登录的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="17d86-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="17d86-118">displayName</span><span class="sxs-lookup"><span data-stu-id="17d86-118">displayName</span></span>|<span data-ttu-id="17d86-119">String</span><span class="sxs-lookup"><span data-stu-id="17d86-119">String</span></span>|<span data-ttu-id="17d86-120">表示用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="17d86-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="17d86-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="17d86-121">isCompliant</span></span>|<span data-ttu-id="17d86-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="17d86-122">Boolean</span></span>|<span data-ttu-id="17d86-123">指示设备是否合规。</span><span class="sxs-lookup"><span data-stu-id="17d86-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="17d86-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="17d86-124">isManaged</span></span>|<span data-ttu-id="17d86-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="17d86-125">Boolean</span></span>|<span data-ttu-id="17d86-126">指示设备是否为托管设备。</span><span class="sxs-lookup"><span data-stu-id="17d86-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="17d86-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="17d86-127">operatingSystem</span></span>|<span data-ttu-id="17d86-128">字符串</span><span class="sxs-lookup"><span data-stu-id="17d86-128">String</span></span>|<span data-ttu-id="17d86-129">指示用于登录的操作系统名称和版本。</span><span class="sxs-lookup"><span data-stu-id="17d86-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="17d86-130">trustType</span><span class="sxs-lookup"><span data-stu-id="17d86-130">trustType</span></span>|<span data-ttu-id="17d86-131">字符串</span><span class="sxs-lookup"><span data-stu-id="17d86-131">String</span></span>|<span data-ttu-id="17d86-132">提供有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="17d86-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17d86-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17d86-133">JSON representation</span></span>

<span data-ttu-id="17d86-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17d86-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
