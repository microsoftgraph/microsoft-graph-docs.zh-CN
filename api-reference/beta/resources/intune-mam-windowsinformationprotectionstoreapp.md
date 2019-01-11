---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3d1f5dfe28928b5cea63c487f322429589938278
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867513"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="13bdd-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="13bdd-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="13bdd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="13bdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13bdd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="13bdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13bdd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="13bdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13bdd-107">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="13bdd-107">Store App for Windows information protection</span></span>

<span data-ttu-id="13bdd-108">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="13bdd-108">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13bdd-109">属性</span><span class="sxs-lookup"><span data-stu-id="13bdd-109">Properties</span></span>
|<span data-ttu-id="13bdd-110">属性</span><span class="sxs-lookup"><span data-stu-id="13bdd-110">Property</span></span>|<span data-ttu-id="13bdd-111">类型</span><span class="sxs-lookup"><span data-stu-id="13bdd-111">Type</span></span>|<span data-ttu-id="13bdd-112">说明</span><span class="sxs-lookup"><span data-stu-id="13bdd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bdd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="13bdd-113">displayName</span></span>|<span data-ttu-id="13bdd-114">String</span><span class="sxs-lookup"><span data-stu-id="13bdd-114">String</span></span>|<span data-ttu-id="13bdd-115">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="13bdd-115">App display name.</span></span> <span data-ttu-id="13bdd-116">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="13bdd-116">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="13bdd-117">description</span><span class="sxs-lookup"><span data-stu-id="13bdd-117">description</span></span>|<span data-ttu-id="13bdd-118">String</span><span class="sxs-lookup"><span data-stu-id="13bdd-118">String</span></span>|<span data-ttu-id="13bdd-119">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="13bdd-119">The app's description.</span></span> <span data-ttu-id="13bdd-120">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="13bdd-120">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="13bdd-121">publisherName</span><span class="sxs-lookup"><span data-stu-id="13bdd-121">publisherName</span></span>|<span data-ttu-id="13bdd-122">String</span><span class="sxs-lookup"><span data-stu-id="13bdd-122">String</span></span>|<span data-ttu-id="13bdd-123">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="13bdd-123">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="13bdd-124">productName</span><span class="sxs-lookup"><span data-stu-id="13bdd-124">productName</span></span>|<span data-ttu-id="13bdd-125">String</span><span class="sxs-lookup"><span data-stu-id="13bdd-125">String</span></span>|<span data-ttu-id="13bdd-126">产品名称。</span><span class="sxs-lookup"><span data-stu-id="13bdd-126">The product name.</span></span> <span data-ttu-id="13bdd-127">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="13bdd-127">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="13bdd-128">denied</span><span class="sxs-lookup"><span data-stu-id="13bdd-128">denied</span></span>|<span data-ttu-id="13bdd-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="13bdd-129">Boolean</span></span>|<span data-ttu-id="13bdd-130">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="13bdd-130">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="13bdd-131">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="13bdd-131">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="13bdd-132">关系</span><span class="sxs-lookup"><span data-stu-id="13bdd-132">Relationships</span></span>
<span data-ttu-id="13bdd-133">无</span><span class="sxs-lookup"><span data-stu-id="13bdd-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13bdd-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13bdd-134">JSON Representation</span></span>
<span data-ttu-id="13bdd-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13bdd-135">Here is a JSON representation of the resource.</span></span>
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





