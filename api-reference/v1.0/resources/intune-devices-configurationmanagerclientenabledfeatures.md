---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ea873333002e543a95746b1168b36a6263277ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091297"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="531d1-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="531d1-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="531d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="531d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="531d1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="531d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="531d1-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="531d1-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="531d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="531d1-107">Properties</span></span>
|<span data-ttu-id="531d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="531d1-108">Property</span></span>|<span data-ttu-id="531d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="531d1-109">Type</span></span>|<span data-ttu-id="531d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="531d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="531d1-111">inventory</span><span class="sxs-lookup"><span data-stu-id="531d1-111">inventory</span></span>|<span data-ttu-id="531d1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-112">Boolean</span></span>|<span data-ttu-id="531d1-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="531d1-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="531d1-114">modernApps</span></span>|<span data-ttu-id="531d1-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-115">Boolean</span></span>|<span data-ttu-id="531d1-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="531d1-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="531d1-117">resourceAccess</span></span>|<span data-ttu-id="531d1-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-118">Boolean</span></span>|<span data-ttu-id="531d1-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="531d1-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="531d1-120">deviceConfiguration</span></span>|<span data-ttu-id="531d1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-121">Boolean</span></span>|<span data-ttu-id="531d1-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="531d1-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="531d1-123">compliancePolicy</span></span>|<span data-ttu-id="531d1-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-124">Boolean</span></span>|<span data-ttu-id="531d1-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="531d1-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="531d1-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="531d1-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="531d1-127">Boolean</span></span>|<span data-ttu-id="531d1-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="531d1-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="531d1-129">关系</span><span class="sxs-lookup"><span data-stu-id="531d1-129">Relationships</span></span>
<span data-ttu-id="531d1-130">无</span><span class="sxs-lookup"><span data-stu-id="531d1-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="531d1-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="531d1-131">JSON Representation</span></span>
<span data-ttu-id="531d1-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="531d1-132">Here is a JSON representation of the resource.</span></span>
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









