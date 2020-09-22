---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a756df15be02544f843e6176677f26ea7e95678
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018701"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="8050f-104">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8050f-104">deviceDetail resource type</span></span>

<span data-ttu-id="8050f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8050f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8050f-106">指示与用于登录的设备相关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="8050f-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="8050f-107">其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。</span><span class="sxs-lookup"><span data-stu-id="8050f-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="8050f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8050f-108">Properties</span></span>

| <span data-ttu-id="8050f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8050f-109">Property</span></span>     | <span data-ttu-id="8050f-110">类型</span><span class="sxs-lookup"><span data-stu-id="8050f-110">Type</span></span>   |<span data-ttu-id="8050f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8050f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8050f-112">浏览器</span><span class="sxs-lookup"><span data-stu-id="8050f-112">browser</span></span>|<span data-ttu-id="8050f-113">String</span><span class="sxs-lookup"><span data-stu-id="8050f-113">String</span></span>|<span data-ttu-id="8050f-114">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="8050f-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="8050f-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="8050f-115">deviceId</span></span>|<span data-ttu-id="8050f-116">String</span><span class="sxs-lookup"><span data-stu-id="8050f-116">String</span></span>|<span data-ttu-id="8050f-117">指用于登录的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="8050f-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="8050f-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8050f-118">displayName</span></span>|<span data-ttu-id="8050f-119">String</span><span class="sxs-lookup"><span data-stu-id="8050f-119">String</span></span>|<span data-ttu-id="8050f-120">表示用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="8050f-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="8050f-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="8050f-121">isCompliant</span></span>|<span data-ttu-id="8050f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="8050f-122">Boolean</span></span>|<span data-ttu-id="8050f-123">指示设备是否合规。</span><span class="sxs-lookup"><span data-stu-id="8050f-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="8050f-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="8050f-124">isManaged</span></span>|<span data-ttu-id="8050f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="8050f-125">Boolean</span></span>|<span data-ttu-id="8050f-126">指示设备是否为托管设备。</span><span class="sxs-lookup"><span data-stu-id="8050f-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="8050f-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8050f-127">operatingSystem</span></span>|<span data-ttu-id="8050f-128">String</span><span class="sxs-lookup"><span data-stu-id="8050f-128">String</span></span>|<span data-ttu-id="8050f-129">指示用于登录的操作系统名称和版本。</span><span class="sxs-lookup"><span data-stu-id="8050f-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="8050f-130">trustType</span><span class="sxs-lookup"><span data-stu-id="8050f-130">trustType</span></span>|<span data-ttu-id="8050f-131">String</span><span class="sxs-lookup"><span data-stu-id="8050f-131">String</span></span>|<span data-ttu-id="8050f-132">提供有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="8050f-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8050f-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8050f-133">JSON representation</span></span>

<span data-ttu-id="8050f-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8050f-134">Here is a JSON representation of the resource.</span></span>

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

