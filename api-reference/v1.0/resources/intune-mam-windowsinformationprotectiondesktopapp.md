---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 994c0dacc4374e9600b2be229efe5e4d5393bb4f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448247"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="c9073-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9073-103">windowsInformationProtectionDesktopApp resource type</span></span>

<span data-ttu-id="c9073-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c9073-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9073-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9073-106">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="c9073-106">Desktop App for Windows information protection</span></span>


<span data-ttu-id="c9073-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9073-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9073-108">Properties</span></span>
|<span data-ttu-id="c9073-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9073-109">Property</span></span>|<span data-ttu-id="c9073-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9073-110">Type</span></span>|<span data-ttu-id="c9073-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9073-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9073-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c9073-112">displayName</span></span>|<span data-ttu-id="c9073-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c9073-113">String</span></span>|<span data-ttu-id="c9073-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="c9073-114">App display name.</span></span> <span data-ttu-id="c9073-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c9073-116">说明</span><span class="sxs-lookup"><span data-stu-id="c9073-116">description</span></span>|<span data-ttu-id="c9073-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c9073-117">String</span></span>|<span data-ttu-id="c9073-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c9073-118">The app's description.</span></span> <span data-ttu-id="c9073-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c9073-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="c9073-120">publisherName</span></span>|<span data-ttu-id="c9073-121">String</span><span class="sxs-lookup"><span data-stu-id="c9073-121">String</span></span>|<span data-ttu-id="c9073-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="c9073-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c9073-123">productName</span><span class="sxs-lookup"><span data-stu-id="c9073-123">productName</span></span>|<span data-ttu-id="c9073-124">String</span><span class="sxs-lookup"><span data-stu-id="c9073-124">String</span></span>|<span data-ttu-id="c9073-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="c9073-125">The product name.</span></span> <span data-ttu-id="c9073-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c9073-127">denied</span><span class="sxs-lookup"><span data-stu-id="c9073-127">denied</span></span>|<span data-ttu-id="c9073-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9073-128">Boolean</span></span>|<span data-ttu-id="c9073-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="c9073-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="c9073-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c9073-131">binaryName</span><span class="sxs-lookup"><span data-stu-id="c9073-131">binaryName</span></span>|<span data-ttu-id="c9073-132">String</span><span class="sxs-lookup"><span data-stu-id="c9073-132">String</span></span>|<span data-ttu-id="c9073-133">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="c9073-133">The binary name.</span></span>|
|<span data-ttu-id="c9073-134">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="c9073-134">binaryVersionLow</span></span>|<span data-ttu-id="c9073-135">String</span><span class="sxs-lookup"><span data-stu-id="c9073-135">String</span></span>|<span data-ttu-id="c9073-136">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="c9073-136">The lower binary version.</span></span>|
|<span data-ttu-id="c9073-137">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="c9073-137">binaryVersionHigh</span></span>|<span data-ttu-id="c9073-138">String</span><span class="sxs-lookup"><span data-stu-id="c9073-138">String</span></span>|<span data-ttu-id="c9073-139">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="c9073-139">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9073-140">关系</span><span class="sxs-lookup"><span data-stu-id="c9073-140">Relationships</span></span>
<span data-ttu-id="c9073-141">无</span><span class="sxs-lookup"><span data-stu-id="c9073-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9073-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9073-142">JSON Representation</span></span>
<span data-ttu-id="c9073-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9073-143">Here is a JSON representation of the resource.</span></span>
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




