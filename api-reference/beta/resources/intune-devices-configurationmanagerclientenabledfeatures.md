---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 07b143a8d61335c44c83d1d88b9a67d2d3c2e4dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962084"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="df8ea-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="df8ea-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="df8ea-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="df8ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df8ea-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df8ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df8ea-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df8ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df8ea-107">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="df8ea-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="df8ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="df8ea-108">Properties</span></span>
|<span data-ttu-id="df8ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="df8ea-109">Property</span></span>|<span data-ttu-id="df8ea-110">类型</span><span class="sxs-lookup"><span data-stu-id="df8ea-110">Type</span></span>|<span data-ttu-id="df8ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="df8ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df8ea-112">inventory</span><span class="sxs-lookup"><span data-stu-id="df8ea-112">inventory</span></span>|<span data-ttu-id="df8ea-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-113">Boolean</span></span>|<span data-ttu-id="df8ea-114">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="df8ea-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="df8ea-115">modernApps</span></span>|<span data-ttu-id="df8ea-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-116">Boolean</span></span>|<span data-ttu-id="df8ea-117">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="df8ea-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="df8ea-118">resourceAccess</span></span>|<span data-ttu-id="df8ea-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-119">Boolean</span></span>|<span data-ttu-id="df8ea-120">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="df8ea-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="df8ea-121">deviceConfiguration</span></span>|<span data-ttu-id="df8ea-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-122">Boolean</span></span>|<span data-ttu-id="df8ea-123">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="df8ea-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="df8ea-124">compliancePolicy</span></span>|<span data-ttu-id="df8ea-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-125">Boolean</span></span>|<span data-ttu-id="df8ea-126">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="df8ea-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="df8ea-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="df8ea-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8ea-128">Boolean</span></span>|<span data-ttu-id="df8ea-129">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="df8ea-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="df8ea-130">关系</span><span class="sxs-lookup"><span data-stu-id="df8ea-130">Relationships</span></span>
<span data-ttu-id="df8ea-131">无</span><span class="sxs-lookup"><span data-stu-id="df8ea-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df8ea-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df8ea-132">JSON Representation</span></span>
<span data-ttu-id="df8ea-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df8ea-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```





