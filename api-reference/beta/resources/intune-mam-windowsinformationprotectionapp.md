---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d44aa233e03a193ea0d061f55748cb0d7319a95b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809588"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="a9371-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9371-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="a9371-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9371-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9371-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9371-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9371-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a9371-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9371-107">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="a9371-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="a9371-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9371-108">Properties</span></span>
|<span data-ttu-id="a9371-109">属性</span><span class="sxs-lookup"><span data-stu-id="a9371-109">Property</span></span>|<span data-ttu-id="a9371-110">类型</span><span class="sxs-lookup"><span data-stu-id="a9371-110">Type</span></span>|<span data-ttu-id="a9371-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9371-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9371-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a9371-112">displayName</span></span>|<span data-ttu-id="a9371-113">String</span><span class="sxs-lookup"><span data-stu-id="a9371-113">String</span></span>|<span data-ttu-id="a9371-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="a9371-114">App display name.</span></span>|
|<span data-ttu-id="a9371-115">description</span><span class="sxs-lookup"><span data-stu-id="a9371-115">description</span></span>|<span data-ttu-id="a9371-116">String</span><span class="sxs-lookup"><span data-stu-id="a9371-116">String</span></span>|<span data-ttu-id="a9371-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a9371-117">The app's description.</span></span>|
|<span data-ttu-id="a9371-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="a9371-118">publisherName</span></span>|<span data-ttu-id="a9371-119">String</span><span class="sxs-lookup"><span data-stu-id="a9371-119">String</span></span>|<span data-ttu-id="a9371-120">发布者名称</span><span class="sxs-lookup"><span data-stu-id="a9371-120">The publisher name</span></span>|
|<span data-ttu-id="a9371-121">productName</span><span class="sxs-lookup"><span data-stu-id="a9371-121">productName</span></span>|<span data-ttu-id="a9371-122">String</span><span class="sxs-lookup"><span data-stu-id="a9371-122">String</span></span>|<span data-ttu-id="a9371-123">产品名称。</span><span class="sxs-lookup"><span data-stu-id="a9371-123">The product name.</span></span>|
|<span data-ttu-id="a9371-124">denied</span><span class="sxs-lookup"><span data-stu-id="a9371-124">denied</span></span>|<span data-ttu-id="a9371-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="a9371-125">Boolean</span></span>|<span data-ttu-id="a9371-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="a9371-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9371-127">关系</span><span class="sxs-lookup"><span data-stu-id="a9371-127">Relationships</span></span>
<span data-ttu-id="a9371-128">无</span><span class="sxs-lookup"><span data-stu-id="a9371-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9371-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9371-129">JSON Representation</span></span>
<span data-ttu-id="a9371-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9371-130">Here is a JSON representation of the resource.</span></span>
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





