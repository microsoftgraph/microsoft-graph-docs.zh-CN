---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e67e76dcec3390f172f4d2819bf7d22ee63f7da5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574430"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="48ea8-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="48ea8-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="48ea8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48ea8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48ea8-105">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="48ea8-105">Store App for Windows information protection</span></span>


<span data-ttu-id="48ea8-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="48ea8-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48ea8-107">属性</span><span class="sxs-lookup"><span data-stu-id="48ea8-107">Properties</span></span>
|<span data-ttu-id="48ea8-108">属性</span><span class="sxs-lookup"><span data-stu-id="48ea8-108">Property</span></span>|<span data-ttu-id="48ea8-109">类型</span><span class="sxs-lookup"><span data-stu-id="48ea8-109">Type</span></span>|<span data-ttu-id="48ea8-110">说明</span><span class="sxs-lookup"><span data-stu-id="48ea8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48ea8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="48ea8-111">displayName</span></span>|<span data-ttu-id="48ea8-112">字符串</span><span class="sxs-lookup"><span data-stu-id="48ea8-112">String</span></span>|<span data-ttu-id="48ea8-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="48ea8-113">App display name.</span></span> <span data-ttu-id="48ea8-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="48ea8-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="48ea8-115">说明</span><span class="sxs-lookup"><span data-stu-id="48ea8-115">description</span></span>|<span data-ttu-id="48ea8-116">String</span><span class="sxs-lookup"><span data-stu-id="48ea8-116">String</span></span>|<span data-ttu-id="48ea8-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="48ea8-117">The app's description.</span></span> <span data-ttu-id="48ea8-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="48ea8-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="48ea8-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="48ea8-119">publisherName</span></span>|<span data-ttu-id="48ea8-120">String</span><span class="sxs-lookup"><span data-stu-id="48ea8-120">String</span></span>|<span data-ttu-id="48ea8-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="48ea8-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="48ea8-122">productName</span><span class="sxs-lookup"><span data-stu-id="48ea8-122">productName</span></span>|<span data-ttu-id="48ea8-123">String</span><span class="sxs-lookup"><span data-stu-id="48ea8-123">String</span></span>|<span data-ttu-id="48ea8-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="48ea8-124">The product name.</span></span> <span data-ttu-id="48ea8-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="48ea8-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="48ea8-126">denied</span><span class="sxs-lookup"><span data-stu-id="48ea8-126">denied</span></span>|<span data-ttu-id="48ea8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="48ea8-127">Boolean</span></span>|<span data-ttu-id="48ea8-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="48ea8-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="48ea8-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="48ea8-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="48ea8-130">关系</span><span class="sxs-lookup"><span data-stu-id="48ea8-130">Relationships</span></span>
<span data-ttu-id="48ea8-131">无</span><span class="sxs-lookup"><span data-stu-id="48ea8-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48ea8-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48ea8-132">JSON Representation</span></span>
<span data-ttu-id="48ea8-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48ea8-133">Here is a JSON representation of the resource.</span></span>
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



