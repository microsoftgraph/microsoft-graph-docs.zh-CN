---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c157357c4ddad0bbdd49e26e2e632ad86c4e41e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752761"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="365e8-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="365e8-103">windowsInformationProtectionDesktopApp resource type</span></span>

<span data-ttu-id="365e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="365e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="365e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365e8-106">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="365e8-106">Desktop App for Windows information protection</span></span>


<span data-ttu-id="365e8-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="365e8-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="365e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="365e8-108">Properties</span></span>
|<span data-ttu-id="365e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="365e8-109">Property</span></span>|<span data-ttu-id="365e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="365e8-110">Type</span></span>|<span data-ttu-id="365e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="365e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365e8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="365e8-112">displayName</span></span>|<span data-ttu-id="365e8-113">String</span><span class="sxs-lookup"><span data-stu-id="365e8-113">String</span></span>|<span data-ttu-id="365e8-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="365e8-114">App display name.</span></span> <span data-ttu-id="365e8-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="365e8-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="365e8-116">说明</span><span class="sxs-lookup"><span data-stu-id="365e8-116">description</span></span>|<span data-ttu-id="365e8-117">String</span><span class="sxs-lookup"><span data-stu-id="365e8-117">String</span></span>|<span data-ttu-id="365e8-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="365e8-118">The app's description.</span></span> <span data-ttu-id="365e8-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="365e8-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="365e8-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="365e8-120">publisherName</span></span>|<span data-ttu-id="365e8-121">String</span><span class="sxs-lookup"><span data-stu-id="365e8-121">String</span></span>|<span data-ttu-id="365e8-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="365e8-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="365e8-123">productName</span><span class="sxs-lookup"><span data-stu-id="365e8-123">productName</span></span>|<span data-ttu-id="365e8-124">String</span><span class="sxs-lookup"><span data-stu-id="365e8-124">String</span></span>|<span data-ttu-id="365e8-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="365e8-125">The product name.</span></span> <span data-ttu-id="365e8-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="365e8-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="365e8-127">denied</span><span class="sxs-lookup"><span data-stu-id="365e8-127">denied</span></span>|<span data-ttu-id="365e8-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="365e8-128">Boolean</span></span>|<span data-ttu-id="365e8-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="365e8-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="365e8-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="365e8-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="365e8-131">binaryName</span><span class="sxs-lookup"><span data-stu-id="365e8-131">binaryName</span></span>|<span data-ttu-id="365e8-132">String</span><span class="sxs-lookup"><span data-stu-id="365e8-132">String</span></span>|<span data-ttu-id="365e8-133">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="365e8-133">The binary name.</span></span>|
|<span data-ttu-id="365e8-134">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="365e8-134">binaryVersionLow</span></span>|<span data-ttu-id="365e8-135">String</span><span class="sxs-lookup"><span data-stu-id="365e8-135">String</span></span>|<span data-ttu-id="365e8-136">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="365e8-136">The lower binary version.</span></span>|
|<span data-ttu-id="365e8-137">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="365e8-137">binaryVersionHigh</span></span>|<span data-ttu-id="365e8-138">String</span><span class="sxs-lookup"><span data-stu-id="365e8-138">String</span></span>|<span data-ttu-id="365e8-139">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="365e8-139">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="365e8-140">关系</span><span class="sxs-lookup"><span data-stu-id="365e8-140">Relationships</span></span>
<span data-ttu-id="365e8-141">无</span><span class="sxs-lookup"><span data-stu-id="365e8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="365e8-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="365e8-142">JSON Representation</span></span>
<span data-ttu-id="365e8-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="365e8-143">Here is a JSON representation of the resource.</span></span>
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




