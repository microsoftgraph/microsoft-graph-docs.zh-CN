---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 其中包括设备浏览器和操作系统等信息, 以及设备是否为 Azure AD 托管。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a6ea50eeea3a906346b69466d2686a2de101792a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629297"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="1cced-104">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cced-104">deviceDetail resource type</span></span>

<span data-ttu-id="1cced-105">指示与用于登录的设备相关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cced-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="1cced-106">其中包括设备浏览器和操作系统等信息, 以及设备是否为 Azure AD 托管。</span><span class="sxs-lookup"><span data-stu-id="1cced-106">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="1cced-107">属性</span><span class="sxs-lookup"><span data-stu-id="1cced-107">Properties</span></span>

| <span data-ttu-id="1cced-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cced-108">Property</span></span>     | <span data-ttu-id="1cced-109">类型</span><span class="sxs-lookup"><span data-stu-id="1cced-109">Type</span></span>   |<span data-ttu-id="1cced-110">说明</span><span class="sxs-lookup"><span data-stu-id="1cced-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cced-111">浏览器</span><span class="sxs-lookup"><span data-stu-id="1cced-111">browser</span></span>|<span data-ttu-id="1cced-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1cced-112">String</span></span>|<span data-ttu-id="1cced-113">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="1cced-113">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="1cced-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="1cced-114">deviceId</span></span>|<span data-ttu-id="1cced-115">String</span><span class="sxs-lookup"><span data-stu-id="1cced-115">String</span></span>|<span data-ttu-id="1cced-116">指用于登录的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="1cced-116">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="1cced-117">displayName</span><span class="sxs-lookup"><span data-stu-id="1cced-117">displayName</span></span>|<span data-ttu-id="1cced-118">String</span><span class="sxs-lookup"><span data-stu-id="1cced-118">String</span></span>|<span data-ttu-id="1cced-119">表示用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="1cced-119">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="1cced-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="1cced-120">isCompliant</span></span>|<span data-ttu-id="1cced-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cced-121">Boolean</span></span>|<span data-ttu-id="1cced-122">指示设备是否合规。</span><span class="sxs-lookup"><span data-stu-id="1cced-122">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="1cced-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="1cced-123">isManaged</span></span>|<span data-ttu-id="1cced-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cced-124">Boolean</span></span>|<span data-ttu-id="1cced-125">指示设备是否为托管设备。</span><span class="sxs-lookup"><span data-stu-id="1cced-125">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="1cced-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1cced-126">operatingSystem</span></span>|<span data-ttu-id="1cced-127">字符串</span><span class="sxs-lookup"><span data-stu-id="1cced-127">String</span></span>|<span data-ttu-id="1cced-128">指示用于登录的操作系统名称和版本。</span><span class="sxs-lookup"><span data-stu-id="1cced-128">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="1cced-129">trustType</span><span class="sxs-lookup"><span data-stu-id="1cced-129">trustType</span></span>|<span data-ttu-id="1cced-130">字符串</span><span class="sxs-lookup"><span data-stu-id="1cced-130">String</span></span>|<span data-ttu-id="1cced-131">提供有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="1cced-131">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1cced-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cced-132">JSON representation</span></span>

<span data-ttu-id="1cced-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cced-133">Here is a JSON representation of the resource.</span></span>

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
