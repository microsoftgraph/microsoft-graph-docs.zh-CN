---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba45dd4f3bb450cfc9822fb68f1b4511f69da2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977386"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="7c0db-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c0db-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="7c0db-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7c0db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c0db-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="7c0db-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="7c0db-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c0db-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c0db-107">属性</span><span class="sxs-lookup"><span data-stu-id="7c0db-107">Properties</span></span>
|<span data-ttu-id="7c0db-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c0db-108">Property</span></span>|<span data-ttu-id="7c0db-109">类型</span><span class="sxs-lookup"><span data-stu-id="7c0db-109">Type</span></span>|<span data-ttu-id="7c0db-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c0db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0db-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7c0db-111">displayName</span></span>|<span data-ttu-id="7c0db-112">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-112">String</span></span>|<span data-ttu-id="7c0db-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c0db-113">App display name.</span></span> <span data-ttu-id="7c0db-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c0db-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7c0db-115">description</span><span class="sxs-lookup"><span data-stu-id="7c0db-115">description</span></span>|<span data-ttu-id="7c0db-116">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-116">String</span></span>|<span data-ttu-id="7c0db-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7c0db-117">The app's description.</span></span> <span data-ttu-id="7c0db-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c0db-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7c0db-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="7c0db-119">publisherName</span></span>|<span data-ttu-id="7c0db-120">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-120">String</span></span>|<span data-ttu-id="7c0db-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="7c0db-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7c0db-122">productName</span><span class="sxs-lookup"><span data-stu-id="7c0db-122">productName</span></span>|<span data-ttu-id="7c0db-123">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-123">String</span></span>|<span data-ttu-id="7c0db-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="7c0db-124">The product name.</span></span> <span data-ttu-id="7c0db-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c0db-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7c0db-126">denied</span><span class="sxs-lookup"><span data-stu-id="7c0db-126">denied</span></span>|<span data-ttu-id="7c0db-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="7c0db-127">Boolean</span></span>|<span data-ttu-id="7c0db-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="7c0db-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="7c0db-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c0db-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="7c0db-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="7c0db-130">binaryName</span></span>|<span data-ttu-id="7c0db-131">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-131">String</span></span>|<span data-ttu-id="7c0db-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="7c0db-132">The binary name.</span></span>|
|<span data-ttu-id="7c0db-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="7c0db-133">binaryVersionLow</span></span>|<span data-ttu-id="7c0db-134">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-134">String</span></span>|<span data-ttu-id="7c0db-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="7c0db-135">The lower binary version.</span></span>|
|<span data-ttu-id="7c0db-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="7c0db-136">binaryVersionHigh</span></span>|<span data-ttu-id="7c0db-137">String</span><span class="sxs-lookup"><span data-stu-id="7c0db-137">String</span></span>|<span data-ttu-id="7c0db-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="7c0db-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0db-139">关系</span><span class="sxs-lookup"><span data-stu-id="7c0db-139">Relationships</span></span>
<span data-ttu-id="7c0db-140">无</span><span class="sxs-lookup"><span data-stu-id="7c0db-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7c0db-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c0db-141">JSON Representation</span></span>
<span data-ttu-id="7c0db-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c0db-142">Here is a JSON representation of the resource.</span></span>
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



