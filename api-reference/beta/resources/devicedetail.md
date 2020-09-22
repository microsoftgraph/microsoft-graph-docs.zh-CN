---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69d8d1e2314021752a5f1a0ab3650d8176ecc8dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049847"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="c5d5f-103">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5d5f-103">deviceDetail resource type</span></span>

<span data-ttu-id="c5d5f-104">命名空间： microsoft. graph 指示与用于登录的设备相关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="c5d5f-105">包括设备浏览器和操作系统信息（如果设备是 Azure AD 托管）等信息。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="c5d5f-106">属性</span><span class="sxs-lookup"><span data-stu-id="c5d5f-106">Properties</span></span>
| <span data-ttu-id="c5d5f-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5d5f-107">Property</span></span>     | <span data-ttu-id="c5d5f-108">类型</span><span class="sxs-lookup"><span data-stu-id="c5d5f-108">Type</span></span>   |<span data-ttu-id="c5d5f-109">说明</span><span class="sxs-lookup"><span data-stu-id="c5d5f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5d5f-110">浏览器</span><span class="sxs-lookup"><span data-stu-id="c5d5f-110">browser</span></span>|<span data-ttu-id="c5d5f-111">String</span><span class="sxs-lookup"><span data-stu-id="c5d5f-111">String</span></span>|<span data-ttu-id="c5d5f-112">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="c5d5f-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="c5d5f-113">deviceId</span></span>|<span data-ttu-id="c5d5f-114">String</span><span class="sxs-lookup"><span data-stu-id="c5d5f-114">String</span></span>|<span data-ttu-id="c5d5f-115">指用于登录的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="c5d5f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d5f-116">displayName</span></span>|<span data-ttu-id="c5d5f-117">String</span><span class="sxs-lookup"><span data-stu-id="c5d5f-117">String</span></span>|<span data-ttu-id="c5d5f-118">指用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="c5d5f-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="c5d5f-119">isCompliant</span></span>|<span data-ttu-id="c5d5f-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d5f-120">Boolean</span></span>|<span data-ttu-id="c5d5f-121">指示设备是否合规。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="c5d5f-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="c5d5f-122">isManaged</span></span>|<span data-ttu-id="c5d5f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5d5f-123">Boolean</span></span>|<span data-ttu-id="c5d5f-124">指示设备是否为托管设备。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="c5d5f-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c5d5f-125">operatingSystem</span></span>|<span data-ttu-id="c5d5f-126">String</span><span class="sxs-lookup"><span data-stu-id="c5d5f-126">String</span></span>|<span data-ttu-id="c5d5f-127">指示用于登录的 OS 名称和版本。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="c5d5f-128">trustType</span><span class="sxs-lookup"><span data-stu-id="c5d5f-128">trustType</span></span>|<span data-ttu-id="c5d5f-129">String</span><span class="sxs-lookup"><span data-stu-id="c5d5f-129">String</span></span>|<span data-ttu-id="c5d5f-130">指示有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5d5f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5d5f-131">JSON representation</span></span>

<span data-ttu-id="c5d5f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5d5f-132">Here is a JSON representation of the resource.</span></span>

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


