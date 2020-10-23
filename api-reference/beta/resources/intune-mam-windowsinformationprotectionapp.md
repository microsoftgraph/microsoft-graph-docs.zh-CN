---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bc6b00185db677901e5e6a888e8b6b8197dfe1b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727279"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="09d88-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="09d88-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="09d88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09d88-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09d88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09d88-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09d88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09d88-107">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="09d88-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="09d88-108">属性</span><span class="sxs-lookup"><span data-stu-id="09d88-108">Properties</span></span>
|<span data-ttu-id="09d88-109">属性</span><span class="sxs-lookup"><span data-stu-id="09d88-109">Property</span></span>|<span data-ttu-id="09d88-110">类型</span><span class="sxs-lookup"><span data-stu-id="09d88-110">Type</span></span>|<span data-ttu-id="09d88-111">说明</span><span class="sxs-lookup"><span data-stu-id="09d88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09d88-112">displayName</span><span class="sxs-lookup"><span data-stu-id="09d88-112">displayName</span></span>|<span data-ttu-id="09d88-113">String</span><span class="sxs-lookup"><span data-stu-id="09d88-113">String</span></span>|<span data-ttu-id="09d88-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="09d88-114">App display name.</span></span>|
|<span data-ttu-id="09d88-115">说明</span><span class="sxs-lookup"><span data-stu-id="09d88-115">description</span></span>|<span data-ttu-id="09d88-116">String</span><span class="sxs-lookup"><span data-stu-id="09d88-116">String</span></span>|<span data-ttu-id="09d88-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="09d88-117">The app's description.</span></span>|
|<span data-ttu-id="09d88-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="09d88-118">publisherName</span></span>|<span data-ttu-id="09d88-119">String</span><span class="sxs-lookup"><span data-stu-id="09d88-119">String</span></span>|<span data-ttu-id="09d88-120">发布者名称</span><span class="sxs-lookup"><span data-stu-id="09d88-120">The publisher name</span></span>|
|<span data-ttu-id="09d88-121">productName</span><span class="sxs-lookup"><span data-stu-id="09d88-121">productName</span></span>|<span data-ttu-id="09d88-122">String</span><span class="sxs-lookup"><span data-stu-id="09d88-122">String</span></span>|<span data-ttu-id="09d88-123">产品名称。</span><span class="sxs-lookup"><span data-stu-id="09d88-123">The product name.</span></span>|
|<span data-ttu-id="09d88-124">denied</span><span class="sxs-lookup"><span data-stu-id="09d88-124">denied</span></span>|<span data-ttu-id="09d88-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="09d88-125">Boolean</span></span>|<span data-ttu-id="09d88-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="09d88-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09d88-127">关系</span><span class="sxs-lookup"><span data-stu-id="09d88-127">Relationships</span></span>
<span data-ttu-id="09d88-128">无</span><span class="sxs-lookup"><span data-stu-id="09d88-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09d88-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09d88-129">JSON Representation</span></span>
<span data-ttu-id="09d88-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09d88-130">Here is a JSON representation of the resource.</span></span>
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





