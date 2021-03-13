---
title: deviceDetail 资源类型
description: 指示与用于登录的设备关联的设备详细信息。
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb6b338793b77e3079922cd8c372e402488a22c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761126"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="0ab42-103">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ab42-103">deviceDetail resource type</span></span>

<span data-ttu-id="0ab42-104">命名空间：microsoft.graph 指示与用于登录的设备关联的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ab42-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="0ab42-105">包括设备浏览器和操作系统信息（如果设备是 Azure AD 托管设备）的信息。</span><span class="sxs-lookup"><span data-stu-id="0ab42-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="0ab42-106">属性</span><span class="sxs-lookup"><span data-stu-id="0ab42-106">Properties</span></span>
| <span data-ttu-id="0ab42-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ab42-107">Property</span></span>     | <span data-ttu-id="0ab42-108">类型</span><span class="sxs-lookup"><span data-stu-id="0ab42-108">Type</span></span>   |<span data-ttu-id="0ab42-109">说明</span><span class="sxs-lookup"><span data-stu-id="0ab42-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ab42-110">浏览器</span><span class="sxs-lookup"><span data-stu-id="0ab42-110">browser</span></span>|<span data-ttu-id="0ab42-111">String</span><span class="sxs-lookup"><span data-stu-id="0ab42-111">String</span></span>|<span data-ttu-id="0ab42-112">指示用于登录的浏览器信息。</span><span class="sxs-lookup"><span data-stu-id="0ab42-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="0ab42-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="0ab42-113">deviceId</span></span>|<span data-ttu-id="0ab42-114">String</span><span class="sxs-lookup"><span data-stu-id="0ab42-114">String</span></span>|<span data-ttu-id="0ab42-115">引用用于登录的设备的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0ab42-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="0ab42-116">displayName</span><span class="sxs-lookup"><span data-stu-id="0ab42-116">displayName</span></span>|<span data-ttu-id="0ab42-117">String</span><span class="sxs-lookup"><span data-stu-id="0ab42-117">String</span></span>|<span data-ttu-id="0ab42-118">指用于登录的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="0ab42-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="0ab42-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="0ab42-119">isCompliant</span></span>|<span data-ttu-id="0ab42-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ab42-120">Boolean</span></span>|<span data-ttu-id="0ab42-121">指示设备是否符合要求。</span><span class="sxs-lookup"><span data-stu-id="0ab42-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="0ab42-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="0ab42-122">isManaged</span></span>|<span data-ttu-id="0ab42-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ab42-123">Boolean</span></span>|<span data-ttu-id="0ab42-124">指示设备是否受管理。</span><span class="sxs-lookup"><span data-stu-id="0ab42-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="0ab42-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0ab42-125">operatingSystem</span></span>|<span data-ttu-id="0ab42-126">String</span><span class="sxs-lookup"><span data-stu-id="0ab42-126">String</span></span>|<span data-ttu-id="0ab42-127">指示用于登录的操作系统名称和版本。</span><span class="sxs-lookup"><span data-stu-id="0ab42-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="0ab42-128">trustType</span><span class="sxs-lookup"><span data-stu-id="0ab42-128">trustType</span></span>|<span data-ttu-id="0ab42-129">String</span><span class="sxs-lookup"><span data-stu-id="0ab42-129">String</span></span>|<span data-ttu-id="0ab42-130">指示已登录设备是否已加入 Workplace、AzureAD Joined、Domain Joined 的信息。</span><span class="sxs-lookup"><span data-stu-id="0ab42-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ab42-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ab42-131">JSON representation</span></span>

<span data-ttu-id="0ab42-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ab42-132">Here is a JSON representation of the resource.</span></span>

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


