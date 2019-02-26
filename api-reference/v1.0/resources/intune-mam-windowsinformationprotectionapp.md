---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257034"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="ddac5-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddac5-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="ddac5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddac5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddac5-105">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="ddac5-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="ddac5-106">属性</span><span class="sxs-lookup"><span data-stu-id="ddac5-106">Properties</span></span>
|<span data-ttu-id="ddac5-107">属性</span><span class="sxs-lookup"><span data-stu-id="ddac5-107">Property</span></span>|<span data-ttu-id="ddac5-108">类型</span><span class="sxs-lookup"><span data-stu-id="ddac5-108">Type</span></span>|<span data-ttu-id="ddac5-109">说明</span><span class="sxs-lookup"><span data-stu-id="ddac5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddac5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ddac5-110">displayName</span></span>|<span data-ttu-id="ddac5-111">String</span><span class="sxs-lookup"><span data-stu-id="ddac5-111">String</span></span>|<span data-ttu-id="ddac5-112">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="ddac5-112">App display name.</span></span>|
|<span data-ttu-id="ddac5-113">description</span><span class="sxs-lookup"><span data-stu-id="ddac5-113">description</span></span>|<span data-ttu-id="ddac5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ddac5-114">String</span></span>|<span data-ttu-id="ddac5-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ddac5-115">The app's description.</span></span>|
|<span data-ttu-id="ddac5-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="ddac5-116">publisherName</span></span>|<span data-ttu-id="ddac5-117">String</span><span class="sxs-lookup"><span data-stu-id="ddac5-117">String</span></span>|<span data-ttu-id="ddac5-118">发布者名称</span><span class="sxs-lookup"><span data-stu-id="ddac5-118">The publisher name</span></span>|
|<span data-ttu-id="ddac5-119">productName</span><span class="sxs-lookup"><span data-stu-id="ddac5-119">productName</span></span>|<span data-ttu-id="ddac5-120">String</span><span class="sxs-lookup"><span data-stu-id="ddac5-120">String</span></span>|<span data-ttu-id="ddac5-121">产品名称。</span><span class="sxs-lookup"><span data-stu-id="ddac5-121">The product name.</span></span>|
|<span data-ttu-id="ddac5-122">denied</span><span class="sxs-lookup"><span data-stu-id="ddac5-122">denied</span></span>|<span data-ttu-id="ddac5-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddac5-123">Boolean</span></span>|<span data-ttu-id="ddac5-124">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="ddac5-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddac5-125">关系</span><span class="sxs-lookup"><span data-stu-id="ddac5-125">Relationships</span></span>
<span data-ttu-id="ddac5-126">无</span><span class="sxs-lookup"><span data-stu-id="ddac5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddac5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddac5-127">JSON Representation</span></span>
<span data-ttu-id="ddac5-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddac5-128">Here is a JSON representation of the resource.</span></span>
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



