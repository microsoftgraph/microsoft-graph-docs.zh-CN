---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264419"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="65680-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="65680-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="65680-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65680-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65680-105">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="65680-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="65680-106">属性</span><span class="sxs-lookup"><span data-stu-id="65680-106">Properties</span></span>
|<span data-ttu-id="65680-107">属性</span><span class="sxs-lookup"><span data-stu-id="65680-107">Property</span></span>|<span data-ttu-id="65680-108">类型</span><span class="sxs-lookup"><span data-stu-id="65680-108">Type</span></span>|<span data-ttu-id="65680-109">说明</span><span class="sxs-lookup"><span data-stu-id="65680-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65680-110">inventory</span><span class="sxs-lookup"><span data-stu-id="65680-110">inventory</span></span>|<span data-ttu-id="65680-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-111">Boolean</span></span>|<span data-ttu-id="65680-112">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="65680-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="65680-113">modernApps</span></span>|<span data-ttu-id="65680-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-114">Boolean</span></span>|<span data-ttu-id="65680-115">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="65680-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="65680-116">resourceAccess</span></span>|<span data-ttu-id="65680-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-117">Boolean</span></span>|<span data-ttu-id="65680-118">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="65680-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="65680-119">deviceConfiguration</span></span>|<span data-ttu-id="65680-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-120">Boolean</span></span>|<span data-ttu-id="65680-121">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="65680-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="65680-122">compliancePolicy</span></span>|<span data-ttu-id="65680-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-123">Boolean</span></span>|<span data-ttu-id="65680-124">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="65680-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="65680-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="65680-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="65680-126">Boolean</span></span>|<span data-ttu-id="65680-127">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="65680-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="65680-128">关系</span><span class="sxs-lookup"><span data-stu-id="65680-128">Relationships</span></span>
<span data-ttu-id="65680-129">无</span><span class="sxs-lookup"><span data-stu-id="65680-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65680-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65680-130">JSON Representation</span></span>
<span data-ttu-id="65680-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65680-131">Here is a JSON representation of the resource.</span></span>
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



