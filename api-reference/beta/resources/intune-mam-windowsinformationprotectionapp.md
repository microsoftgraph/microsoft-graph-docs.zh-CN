---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45d428ee18e92e76f5a13c568373219f904fd886
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403684"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="02180-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="02180-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="02180-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="02180-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="02180-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02180-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02180-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02180-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02180-107">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="02180-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="02180-108">属性</span><span class="sxs-lookup"><span data-stu-id="02180-108">Properties</span></span>
|<span data-ttu-id="02180-109">属性</span><span class="sxs-lookup"><span data-stu-id="02180-109">Property</span></span>|<span data-ttu-id="02180-110">类型</span><span class="sxs-lookup"><span data-stu-id="02180-110">Type</span></span>|<span data-ttu-id="02180-111">说明</span><span class="sxs-lookup"><span data-stu-id="02180-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02180-112">displayName</span><span class="sxs-lookup"><span data-stu-id="02180-112">displayName</span></span>|<span data-ttu-id="02180-113">String</span><span class="sxs-lookup"><span data-stu-id="02180-113">String</span></span>|<span data-ttu-id="02180-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="02180-114">App display name.</span></span>|
|<span data-ttu-id="02180-115">description</span><span class="sxs-lookup"><span data-stu-id="02180-115">description</span></span>|<span data-ttu-id="02180-116">String</span><span class="sxs-lookup"><span data-stu-id="02180-116">String</span></span>|<span data-ttu-id="02180-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="02180-117">The app's description.</span></span>|
|<span data-ttu-id="02180-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="02180-118">publisherName</span></span>|<span data-ttu-id="02180-119">String</span><span class="sxs-lookup"><span data-stu-id="02180-119">String</span></span>|<span data-ttu-id="02180-120">发布者名称</span><span class="sxs-lookup"><span data-stu-id="02180-120">The publisher name</span></span>|
|<span data-ttu-id="02180-121">productName</span><span class="sxs-lookup"><span data-stu-id="02180-121">productName</span></span>|<span data-ttu-id="02180-122">String</span><span class="sxs-lookup"><span data-stu-id="02180-122">String</span></span>|<span data-ttu-id="02180-123">产品名称。</span><span class="sxs-lookup"><span data-stu-id="02180-123">The product name.</span></span>|
|<span data-ttu-id="02180-124">denied</span><span class="sxs-lookup"><span data-stu-id="02180-124">denied</span></span>|<span data-ttu-id="02180-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="02180-125">Boolean</span></span>|<span data-ttu-id="02180-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="02180-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02180-127">关系</span><span class="sxs-lookup"><span data-stu-id="02180-127">Relationships</span></span>
<span data-ttu-id="02180-128">无</span><span class="sxs-lookup"><span data-stu-id="02180-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02180-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02180-129">JSON Representation</span></span>
<span data-ttu-id="02180-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02180-130">Here is a JSON representation of the resource.</span></span>
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




