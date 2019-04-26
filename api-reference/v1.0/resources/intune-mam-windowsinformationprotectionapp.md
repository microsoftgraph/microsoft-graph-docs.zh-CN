---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561200"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="f0281-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0281-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="f0281-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0281-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0281-105">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="f0281-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="f0281-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0281-106">Properties</span></span>
|<span data-ttu-id="f0281-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0281-107">Property</span></span>|<span data-ttu-id="f0281-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0281-108">Type</span></span>|<span data-ttu-id="f0281-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0281-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0281-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f0281-110">displayName</span></span>|<span data-ttu-id="f0281-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f0281-111">String</span></span>|<span data-ttu-id="f0281-112">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="f0281-112">App display name.</span></span>|
|<span data-ttu-id="f0281-113">description</span><span class="sxs-lookup"><span data-stu-id="f0281-113">description</span></span>|<span data-ttu-id="f0281-114">String</span><span class="sxs-lookup"><span data-stu-id="f0281-114">String</span></span>|<span data-ttu-id="f0281-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f0281-115">The app's description.</span></span>|
|<span data-ttu-id="f0281-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="f0281-116">publisherName</span></span>|<span data-ttu-id="f0281-117">String</span><span class="sxs-lookup"><span data-stu-id="f0281-117">String</span></span>|<span data-ttu-id="f0281-118">发布者名称</span><span class="sxs-lookup"><span data-stu-id="f0281-118">The publisher name</span></span>|
|<span data-ttu-id="f0281-119">productName</span><span class="sxs-lookup"><span data-stu-id="f0281-119">productName</span></span>|<span data-ttu-id="f0281-120">String</span><span class="sxs-lookup"><span data-stu-id="f0281-120">String</span></span>|<span data-ttu-id="f0281-121">产品名称。</span><span class="sxs-lookup"><span data-stu-id="f0281-121">The product name.</span></span>|
|<span data-ttu-id="f0281-122">denied</span><span class="sxs-lookup"><span data-stu-id="f0281-122">denied</span></span>|<span data-ttu-id="f0281-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0281-123">Boolean</span></span>|<span data-ttu-id="f0281-124">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="f0281-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0281-125">关系</span><span class="sxs-lookup"><span data-stu-id="f0281-125">Relationships</span></span>
<span data-ttu-id="f0281-126">无</span><span class="sxs-lookup"><span data-stu-id="f0281-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0281-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0281-127">JSON Representation</span></span>
<span data-ttu-id="f0281-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0281-128">Here is a JSON representation of the resource.</span></span>
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



