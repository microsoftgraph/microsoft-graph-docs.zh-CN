---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59360d948865e184abab7b9749c764a43b2710d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030057"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="4f95b-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f95b-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="4f95b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f95b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f95b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f95b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f95b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f95b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f95b-107">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="4f95b-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="4f95b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f95b-108">Properties</span></span>
|<span data-ttu-id="4f95b-109">属性</span><span class="sxs-lookup"><span data-stu-id="4f95b-109">Property</span></span>|<span data-ttu-id="4f95b-110">类型</span><span class="sxs-lookup"><span data-stu-id="4f95b-110">Type</span></span>|<span data-ttu-id="4f95b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f95b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f95b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4f95b-112">displayName</span></span>|<span data-ttu-id="4f95b-113">String</span><span class="sxs-lookup"><span data-stu-id="4f95b-113">String</span></span>|<span data-ttu-id="4f95b-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f95b-114">App display name.</span></span>|
|<span data-ttu-id="4f95b-115">description</span><span class="sxs-lookup"><span data-stu-id="4f95b-115">description</span></span>|<span data-ttu-id="4f95b-116">String</span><span class="sxs-lookup"><span data-stu-id="4f95b-116">String</span></span>|<span data-ttu-id="4f95b-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="4f95b-117">The app's description.</span></span>|
|<span data-ttu-id="4f95b-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="4f95b-118">publisherName</span></span>|<span data-ttu-id="4f95b-119">String</span><span class="sxs-lookup"><span data-stu-id="4f95b-119">String</span></span>|<span data-ttu-id="4f95b-120">发布者名称</span><span class="sxs-lookup"><span data-stu-id="4f95b-120">The publisher name</span></span>|
|<span data-ttu-id="4f95b-121">productName</span><span class="sxs-lookup"><span data-stu-id="4f95b-121">productName</span></span>|<span data-ttu-id="4f95b-122">String</span><span class="sxs-lookup"><span data-stu-id="4f95b-122">String</span></span>|<span data-ttu-id="4f95b-123">产品名称。</span><span class="sxs-lookup"><span data-stu-id="4f95b-123">The product name.</span></span>|
|<span data-ttu-id="4f95b-124">denied</span><span class="sxs-lookup"><span data-stu-id="4f95b-124">denied</span></span>|<span data-ttu-id="4f95b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f95b-125">Boolean</span></span>|<span data-ttu-id="4f95b-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="4f95b-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f95b-127">关系</span><span class="sxs-lookup"><span data-stu-id="4f95b-127">Relationships</span></span>
<span data-ttu-id="4f95b-128">无</span><span class="sxs-lookup"><span data-stu-id="4f95b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f95b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f95b-129">JSON Representation</span></span>
<span data-ttu-id="4f95b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f95b-130">Here is a JSON representation of the resource.</span></span>
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






