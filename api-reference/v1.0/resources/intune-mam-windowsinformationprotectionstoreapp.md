---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c15becc47164fd57bbe3d157e9732531a20ebaff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459677"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="23c59-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="23c59-103">windowsInformationProtectionStoreApp resource type</span></span>

<span data-ttu-id="23c59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23c59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23c59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23c59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23c59-106">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="23c59-106">Store App for Windows information protection</span></span>


<span data-ttu-id="23c59-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="23c59-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23c59-108">属性</span><span class="sxs-lookup"><span data-stu-id="23c59-108">Properties</span></span>
|<span data-ttu-id="23c59-109">属性</span><span class="sxs-lookup"><span data-stu-id="23c59-109">Property</span></span>|<span data-ttu-id="23c59-110">类型</span><span class="sxs-lookup"><span data-stu-id="23c59-110">Type</span></span>|<span data-ttu-id="23c59-111">说明</span><span class="sxs-lookup"><span data-stu-id="23c59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c59-112">displayName</span><span class="sxs-lookup"><span data-stu-id="23c59-112">displayName</span></span>|<span data-ttu-id="23c59-113">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-113">String</span></span>|<span data-ttu-id="23c59-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="23c59-114">App display name.</span></span> <span data-ttu-id="23c59-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="23c59-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="23c59-116">description</span><span class="sxs-lookup"><span data-stu-id="23c59-116">description</span></span>|<span data-ttu-id="23c59-117">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-117">String</span></span>|<span data-ttu-id="23c59-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="23c59-118">The app's description.</span></span> <span data-ttu-id="23c59-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="23c59-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="23c59-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="23c59-120">publisherName</span></span>|<span data-ttu-id="23c59-121">String</span><span class="sxs-lookup"><span data-stu-id="23c59-121">String</span></span>|<span data-ttu-id="23c59-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="23c59-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="23c59-123">productName</span><span class="sxs-lookup"><span data-stu-id="23c59-123">productName</span></span>|<span data-ttu-id="23c59-124">String</span><span class="sxs-lookup"><span data-stu-id="23c59-124">String</span></span>|<span data-ttu-id="23c59-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="23c59-125">The product name.</span></span> <span data-ttu-id="23c59-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="23c59-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="23c59-127">denied</span><span class="sxs-lookup"><span data-stu-id="23c59-127">denied</span></span>|<span data-ttu-id="23c59-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="23c59-128">Boolean</span></span>|<span data-ttu-id="23c59-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="23c59-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="23c59-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="23c59-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="23c59-131">关系</span><span class="sxs-lookup"><span data-stu-id="23c59-131">Relationships</span></span>
<span data-ttu-id="23c59-132">无</span><span class="sxs-lookup"><span data-stu-id="23c59-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23c59-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23c59-133">JSON Representation</span></span>
<span data-ttu-id="23c59-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23c59-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```







