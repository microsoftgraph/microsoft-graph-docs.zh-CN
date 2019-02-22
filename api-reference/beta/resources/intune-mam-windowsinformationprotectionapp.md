---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2b8739fd045d4b8e6293164fc7e9b14154a475c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139282"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="e3e8c-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3e8c-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="e3e8c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3e8c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e8c-106">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="e3e8c-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="e3e8c-107">属性</span><span class="sxs-lookup"><span data-stu-id="e3e8c-107">Properties</span></span>
|<span data-ttu-id="e3e8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3e8c-108">Property</span></span>|<span data-ttu-id="e3e8c-109">类型</span><span class="sxs-lookup"><span data-stu-id="e3e8c-109">Type</span></span>|<span data-ttu-id="e3e8c-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3e8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e8c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e8c-111">displayName</span></span>|<span data-ttu-id="e3e8c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e3e8c-112">String</span></span>|<span data-ttu-id="e3e8c-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-113">App display name.</span></span>|
|<span data-ttu-id="e3e8c-114">description</span><span class="sxs-lookup"><span data-stu-id="e3e8c-114">description</span></span>|<span data-ttu-id="e3e8c-115">字符串</span><span class="sxs-lookup"><span data-stu-id="e3e8c-115">String</span></span>|<span data-ttu-id="e3e8c-116">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-116">The app's description.</span></span>|
|<span data-ttu-id="e3e8c-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="e3e8c-117">publisherName</span></span>|<span data-ttu-id="e3e8c-118">String</span><span class="sxs-lookup"><span data-stu-id="e3e8c-118">String</span></span>|<span data-ttu-id="e3e8c-119">发布者名称</span><span class="sxs-lookup"><span data-stu-id="e3e8c-119">The publisher name</span></span>|
|<span data-ttu-id="e3e8c-120">productName</span><span class="sxs-lookup"><span data-stu-id="e3e8c-120">productName</span></span>|<span data-ttu-id="e3e8c-121">String</span><span class="sxs-lookup"><span data-stu-id="e3e8c-121">String</span></span>|<span data-ttu-id="e3e8c-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-122">The product name.</span></span>|
|<span data-ttu-id="e3e8c-123">denied</span><span class="sxs-lookup"><span data-stu-id="e3e8c-123">denied</span></span>|<span data-ttu-id="e3e8c-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3e8c-124">Boolean</span></span>|<span data-ttu-id="e3e8c-125">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3e8c-126">关系</span><span class="sxs-lookup"><span data-stu-id="e3e8c-126">Relationships</span></span>
<span data-ttu-id="e3e8c-127">无</span><span class="sxs-lookup"><span data-stu-id="e3e8c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3e8c-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3e8c-128">JSON Representation</span></span>
<span data-ttu-id="e3e8c-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3e8c-129">Here is a JSON representation of the resource.</span></span>
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




