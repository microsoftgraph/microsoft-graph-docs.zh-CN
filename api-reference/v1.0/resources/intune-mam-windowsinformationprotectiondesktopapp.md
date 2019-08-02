---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d9187858aa90480ba8720bc2111f3ba071492e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037700"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="85511-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="85511-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="85511-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85511-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85511-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="85511-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="85511-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="85511-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85511-107">属性</span><span class="sxs-lookup"><span data-stu-id="85511-107">Properties</span></span>
|<span data-ttu-id="85511-108">属性</span><span class="sxs-lookup"><span data-stu-id="85511-108">Property</span></span>|<span data-ttu-id="85511-109">类型</span><span class="sxs-lookup"><span data-stu-id="85511-109">Type</span></span>|<span data-ttu-id="85511-110">说明</span><span class="sxs-lookup"><span data-stu-id="85511-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85511-111">displayName</span><span class="sxs-lookup"><span data-stu-id="85511-111">displayName</span></span>|<span data-ttu-id="85511-112">字符串</span><span class="sxs-lookup"><span data-stu-id="85511-112">String</span></span>|<span data-ttu-id="85511-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="85511-113">App display name.</span></span> <span data-ttu-id="85511-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="85511-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="85511-115">说明</span><span class="sxs-lookup"><span data-stu-id="85511-115">description</span></span>|<span data-ttu-id="85511-116">字符串</span><span class="sxs-lookup"><span data-stu-id="85511-116">String</span></span>|<span data-ttu-id="85511-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="85511-117">The app's description.</span></span> <span data-ttu-id="85511-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="85511-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="85511-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="85511-119">publisherName</span></span>|<span data-ttu-id="85511-120">String</span><span class="sxs-lookup"><span data-stu-id="85511-120">String</span></span>|<span data-ttu-id="85511-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="85511-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="85511-122">productName</span><span class="sxs-lookup"><span data-stu-id="85511-122">productName</span></span>|<span data-ttu-id="85511-123">String</span><span class="sxs-lookup"><span data-stu-id="85511-123">String</span></span>|<span data-ttu-id="85511-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="85511-124">The product name.</span></span> <span data-ttu-id="85511-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="85511-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="85511-126">denied</span><span class="sxs-lookup"><span data-stu-id="85511-126">denied</span></span>|<span data-ttu-id="85511-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="85511-127">Boolean</span></span>|<span data-ttu-id="85511-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="85511-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="85511-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="85511-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="85511-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="85511-130">binaryName</span></span>|<span data-ttu-id="85511-131">String</span><span class="sxs-lookup"><span data-stu-id="85511-131">String</span></span>|<span data-ttu-id="85511-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="85511-132">The binary name.</span></span>|
|<span data-ttu-id="85511-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="85511-133">binaryVersionLow</span></span>|<span data-ttu-id="85511-134">String</span><span class="sxs-lookup"><span data-stu-id="85511-134">String</span></span>|<span data-ttu-id="85511-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="85511-135">The lower binary version.</span></span>|
|<span data-ttu-id="85511-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="85511-136">binaryVersionHigh</span></span>|<span data-ttu-id="85511-137">String</span><span class="sxs-lookup"><span data-stu-id="85511-137">String</span></span>|<span data-ttu-id="85511-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="85511-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85511-139">关系</span><span class="sxs-lookup"><span data-stu-id="85511-139">Relationships</span></span>
<span data-ttu-id="85511-140">无</span><span class="sxs-lookup"><span data-stu-id="85511-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85511-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85511-141">JSON Representation</span></span>
<span data-ttu-id="85511-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85511-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



