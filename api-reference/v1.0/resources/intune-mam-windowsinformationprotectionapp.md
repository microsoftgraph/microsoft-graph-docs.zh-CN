---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4a64b1b91df7bc52fbec718e0bc5fb13beae308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468479"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="938e6-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="938e6-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="938e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="938e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="938e6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="938e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="938e6-106">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="938e6-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="938e6-107">属性</span><span class="sxs-lookup"><span data-stu-id="938e6-107">Properties</span></span>
|<span data-ttu-id="938e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="938e6-108">Property</span></span>|<span data-ttu-id="938e6-109">类型</span><span class="sxs-lookup"><span data-stu-id="938e6-109">Type</span></span>|<span data-ttu-id="938e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="938e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="938e6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="938e6-111">displayName</span></span>|<span data-ttu-id="938e6-112">字符串</span><span class="sxs-lookup"><span data-stu-id="938e6-112">String</span></span>|<span data-ttu-id="938e6-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="938e6-113">App display name.</span></span>|
|<span data-ttu-id="938e6-114">description</span><span class="sxs-lookup"><span data-stu-id="938e6-114">description</span></span>|<span data-ttu-id="938e6-115">字符串</span><span class="sxs-lookup"><span data-stu-id="938e6-115">String</span></span>|<span data-ttu-id="938e6-116">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="938e6-116">The app's description.</span></span>|
|<span data-ttu-id="938e6-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="938e6-117">publisherName</span></span>|<span data-ttu-id="938e6-118">String</span><span class="sxs-lookup"><span data-stu-id="938e6-118">String</span></span>|<span data-ttu-id="938e6-119">发布者名称</span><span class="sxs-lookup"><span data-stu-id="938e6-119">The publisher name</span></span>|
|<span data-ttu-id="938e6-120">productName</span><span class="sxs-lookup"><span data-stu-id="938e6-120">productName</span></span>|<span data-ttu-id="938e6-121">String</span><span class="sxs-lookup"><span data-stu-id="938e6-121">String</span></span>|<span data-ttu-id="938e6-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="938e6-122">The product name.</span></span>|
|<span data-ttu-id="938e6-123">denied</span><span class="sxs-lookup"><span data-stu-id="938e6-123">denied</span></span>|<span data-ttu-id="938e6-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="938e6-124">Boolean</span></span>|<span data-ttu-id="938e6-125">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="938e6-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="938e6-126">关系</span><span class="sxs-lookup"><span data-stu-id="938e6-126">Relationships</span></span>
<span data-ttu-id="938e6-127">无</span><span class="sxs-lookup"><span data-stu-id="938e6-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="938e6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="938e6-128">JSON Representation</span></span>
<span data-ttu-id="938e6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="938e6-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```







