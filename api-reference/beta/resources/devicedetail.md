---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 包括设备浏览器和操作系统信息 (如果设备是 Azure AD 托管) 等信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3a0d7f141723beb5194860b025fe6fa349eb95a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657698"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="380c6-104">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="380c6-104">deviceDetail resource type</span></span>
<span data-ttu-id="380c6-105">指示与用于登录的设备相关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="380c6-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="380c6-106">包括设备浏览器和操作系统信息 (如果设备是 Azure AD 托管) 等信息。</span><span class="sxs-lookup"><span data-stu-id="380c6-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="380c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="380c6-107">Properties</span></span>
| <span data-ttu-id="380c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="380c6-108">Property</span></span>     | <span data-ttu-id="380c6-109">类型</span><span class="sxs-lookup"><span data-stu-id="380c6-109">Type</span></span>   |<span data-ttu-id="380c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="380c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="380c6-111">浏览器</span><span class="sxs-lookup"><span data-stu-id="380c6-111">browser</span></span>|<span data-ttu-id="380c6-112">String</span><span class="sxs-lookup"><span data-stu-id="380c6-112">String</span></span>|<span data-ttu-id="380c6-113">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="380c6-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="380c6-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="380c6-114">deviceId</span></span>|<span data-ttu-id="380c6-115">String</span><span class="sxs-lookup"><span data-stu-id="380c6-115">String</span></span>|<span data-ttu-id="380c6-116">指用于登录的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="380c6-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="380c6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="380c6-117">displayName</span></span>|<span data-ttu-id="380c6-118">String</span><span class="sxs-lookup"><span data-stu-id="380c6-118">String</span></span>|<span data-ttu-id="380c6-119">指用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="380c6-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="380c6-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="380c6-120">isCompliant</span></span>|<span data-ttu-id="380c6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="380c6-121">Boolean</span></span>|<span data-ttu-id="380c6-122">指示设备是否合规。</span><span class="sxs-lookup"><span data-stu-id="380c6-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="380c6-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="380c6-123">isManaged</span></span>|<span data-ttu-id="380c6-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="380c6-124">Boolean</span></span>|<span data-ttu-id="380c6-125">指示设备是否为托管设备。</span><span class="sxs-lookup"><span data-stu-id="380c6-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="380c6-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="380c6-126">operatingSystem</span></span>|<span data-ttu-id="380c6-127">String</span><span class="sxs-lookup"><span data-stu-id="380c6-127">String</span></span>|<span data-ttu-id="380c6-128">指示用于登录的 OS 名称和版本。</span><span class="sxs-lookup"><span data-stu-id="380c6-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="380c6-129">trustType</span><span class="sxs-lookup"><span data-stu-id="380c6-129">trustType</span></span>|<span data-ttu-id="380c6-130">String</span><span class="sxs-lookup"><span data-stu-id="380c6-130">String</span></span>|<span data-ttu-id="380c6-131">指示有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="380c6-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="380c6-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="380c6-132">JSON representation</span></span>

<span data-ttu-id="380c6-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="380c6-133">Here is a JSON representation of the resource.</span></span>

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
