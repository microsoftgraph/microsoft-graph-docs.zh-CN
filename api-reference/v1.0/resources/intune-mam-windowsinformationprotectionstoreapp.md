---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e78aa854b15763cade9a4d6020f1737bbca1642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814474"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="30529-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="30529-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="30529-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30529-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30529-105">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="30529-105">Store App for Windows information protection</span></span>

<span data-ttu-id="30529-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="30529-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30529-107">属性</span><span class="sxs-lookup"><span data-stu-id="30529-107">Properties</span></span>
|<span data-ttu-id="30529-108">属性</span><span class="sxs-lookup"><span data-stu-id="30529-108">Property</span></span>|<span data-ttu-id="30529-109">类型</span><span class="sxs-lookup"><span data-stu-id="30529-109">Type</span></span>|<span data-ttu-id="30529-110">说明</span><span class="sxs-lookup"><span data-stu-id="30529-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30529-111">displayName</span><span class="sxs-lookup"><span data-stu-id="30529-111">displayName</span></span>|<span data-ttu-id="30529-112">String</span><span class="sxs-lookup"><span data-stu-id="30529-112">String</span></span>|<span data-ttu-id="30529-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="30529-113">App display name.</span></span> <span data-ttu-id="30529-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="30529-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="30529-115">description</span><span class="sxs-lookup"><span data-stu-id="30529-115">description</span></span>|<span data-ttu-id="30529-116">String</span><span class="sxs-lookup"><span data-stu-id="30529-116">String</span></span>|<span data-ttu-id="30529-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="30529-117">The app's description.</span></span> <span data-ttu-id="30529-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="30529-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="30529-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="30529-119">publisherName</span></span>|<span data-ttu-id="30529-120">String</span><span class="sxs-lookup"><span data-stu-id="30529-120">String</span></span>|<span data-ttu-id="30529-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="30529-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="30529-122">productName</span><span class="sxs-lookup"><span data-stu-id="30529-122">productName</span></span>|<span data-ttu-id="30529-123">String</span><span class="sxs-lookup"><span data-stu-id="30529-123">String</span></span>|<span data-ttu-id="30529-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="30529-124">The product name.</span></span> <span data-ttu-id="30529-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="30529-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="30529-126">denied</span><span class="sxs-lookup"><span data-stu-id="30529-126">denied</span></span>|<span data-ttu-id="30529-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="30529-127">Boolean</span></span>|<span data-ttu-id="30529-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="30529-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="30529-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="30529-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="30529-130">关系</span><span class="sxs-lookup"><span data-stu-id="30529-130">Relationships</span></span>
<span data-ttu-id="30529-131">无</span><span class="sxs-lookup"><span data-stu-id="30529-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30529-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30529-132">JSON Representation</span></span>
<span data-ttu-id="30529-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30529-133">Here is a JSON representation of the resource.</span></span>
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



