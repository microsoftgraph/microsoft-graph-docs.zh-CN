---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9517bb807ad257ddba94b991223b781e91bbbc68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890088"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="bd267-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd267-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="bd267-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd267-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd267-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd267-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd267-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd267-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd267-107">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="bd267-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="bd267-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd267-108">Properties</span></span>
|<span data-ttu-id="bd267-109">属性</span><span class="sxs-lookup"><span data-stu-id="bd267-109">Property</span></span>|<span data-ttu-id="bd267-110">类型</span><span class="sxs-lookup"><span data-stu-id="bd267-110">Type</span></span>|<span data-ttu-id="bd267-111">说明</span><span class="sxs-lookup"><span data-stu-id="bd267-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd267-112">inventory</span><span class="sxs-lookup"><span data-stu-id="bd267-112">inventory</span></span>|<span data-ttu-id="bd267-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-113">Boolean</span></span>|<span data-ttu-id="bd267-114">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="bd267-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="bd267-115">modernApps</span></span>|<span data-ttu-id="bd267-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-116">Boolean</span></span>|<span data-ttu-id="bd267-117">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="bd267-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="bd267-118">resourceAccess</span></span>|<span data-ttu-id="bd267-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-119">Boolean</span></span>|<span data-ttu-id="bd267-120">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="bd267-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd267-121">deviceConfiguration</span></span>|<span data-ttu-id="bd267-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-122">Boolean</span></span>|<span data-ttu-id="bd267-123">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="bd267-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bd267-124">compliancePolicy</span></span>|<span data-ttu-id="bd267-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-125">Boolean</span></span>|<span data-ttu-id="bd267-126">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="bd267-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="bd267-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="bd267-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd267-128">Boolean</span></span>|<span data-ttu-id="bd267-129">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="bd267-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd267-130">关系</span><span class="sxs-lookup"><span data-stu-id="bd267-130">Relationships</span></span>
<span data-ttu-id="bd267-131">无</span><span class="sxs-lookup"><span data-stu-id="bd267-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd267-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd267-132">JSON Representation</span></span>
<span data-ttu-id="bd267-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd267-133">Here is a JSON representation of the resource.</span></span>
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





