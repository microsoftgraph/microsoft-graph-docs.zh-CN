---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83ad9e3e500ab5276e4643055f602e763de34fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564251"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="eb966-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb966-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="eb966-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb966-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb966-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="eb966-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="eb966-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb966-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb966-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb966-107">Properties</span></span>
|<span data-ttu-id="eb966-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb966-108">Property</span></span>|<span data-ttu-id="eb966-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb966-109">Type</span></span>|<span data-ttu-id="eb966-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb966-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb966-111">displayName</span><span class="sxs-lookup"><span data-stu-id="eb966-111">displayName</span></span>|<span data-ttu-id="eb966-112">字符串</span><span class="sxs-lookup"><span data-stu-id="eb966-112">String</span></span>|<span data-ttu-id="eb966-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb966-113">App display name.</span></span> <span data-ttu-id="eb966-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb966-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb966-115">说明</span><span class="sxs-lookup"><span data-stu-id="eb966-115">description</span></span>|<span data-ttu-id="eb966-116">String</span><span class="sxs-lookup"><span data-stu-id="eb966-116">String</span></span>|<span data-ttu-id="eb966-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="eb966-117">The app's description.</span></span> <span data-ttu-id="eb966-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb966-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb966-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="eb966-119">publisherName</span></span>|<span data-ttu-id="eb966-120">String</span><span class="sxs-lookup"><span data-stu-id="eb966-120">String</span></span>|<span data-ttu-id="eb966-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="eb966-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb966-122">productName</span><span class="sxs-lookup"><span data-stu-id="eb966-122">productName</span></span>|<span data-ttu-id="eb966-123">String</span><span class="sxs-lookup"><span data-stu-id="eb966-123">String</span></span>|<span data-ttu-id="eb966-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="eb966-124">The product name.</span></span> <span data-ttu-id="eb966-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb966-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb966-126">denied</span><span class="sxs-lookup"><span data-stu-id="eb966-126">denied</span></span>|<span data-ttu-id="eb966-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb966-127">Boolean</span></span>|<span data-ttu-id="eb966-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="eb966-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="eb966-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb966-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb966-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="eb966-130">binaryName</span></span>|<span data-ttu-id="eb966-131">String</span><span class="sxs-lookup"><span data-stu-id="eb966-131">String</span></span>|<span data-ttu-id="eb966-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="eb966-132">The binary name.</span></span>|
|<span data-ttu-id="eb966-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="eb966-133">binaryVersionLow</span></span>|<span data-ttu-id="eb966-134">String</span><span class="sxs-lookup"><span data-stu-id="eb966-134">String</span></span>|<span data-ttu-id="eb966-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="eb966-135">The lower binary version.</span></span>|
|<span data-ttu-id="eb966-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="eb966-136">binaryVersionHigh</span></span>|<span data-ttu-id="eb966-137">String</span><span class="sxs-lookup"><span data-stu-id="eb966-137">String</span></span>|<span data-ttu-id="eb966-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="eb966-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb966-139">关系</span><span class="sxs-lookup"><span data-stu-id="eb966-139">Relationships</span></span>
<span data-ttu-id="eb966-140">无</span><span class="sxs-lookup"><span data-stu-id="eb966-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb966-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb966-141">JSON Representation</span></span>
<span data-ttu-id="eb966-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb966-142">Here is a JSON representation of the resource.</span></span>
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



