---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9d7cab901b78eb980a3617735e94a892f11d634
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751697"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="7df76-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="7df76-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="7df76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7df76-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7df76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df76-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="7df76-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="7df76-107">属性</span><span class="sxs-lookup"><span data-stu-id="7df76-107">Properties</span></span>
|<span data-ttu-id="7df76-108">属性</span><span class="sxs-lookup"><span data-stu-id="7df76-108">Property</span></span>|<span data-ttu-id="7df76-109">类型</span><span class="sxs-lookup"><span data-stu-id="7df76-109">Type</span></span>|<span data-ttu-id="7df76-110">Description</span><span class="sxs-lookup"><span data-stu-id="7df76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df76-111">inventory</span><span class="sxs-lookup"><span data-stu-id="7df76-111">inventory</span></span>|<span data-ttu-id="7df76-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-112">Boolean</span></span>|<span data-ttu-id="7df76-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="7df76-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="7df76-114">modernApps</span></span>|<span data-ttu-id="7df76-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-115">Boolean</span></span>|<span data-ttu-id="7df76-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="7df76-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="7df76-117">resourceAccess</span></span>|<span data-ttu-id="7df76-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-118">Boolean</span></span>|<span data-ttu-id="7df76-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="7df76-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7df76-120">deviceConfiguration</span></span>|<span data-ttu-id="7df76-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-121">Boolean</span></span>|<span data-ttu-id="7df76-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="7df76-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7df76-123">compliancePolicy</span></span>|<span data-ttu-id="7df76-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-124">Boolean</span></span>|<span data-ttu-id="7df76-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="7df76-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="7df76-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="7df76-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df76-127">Boolean</span></span>|<span data-ttu-id="7df76-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="7df76-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df76-129">关系</span><span class="sxs-lookup"><span data-stu-id="7df76-129">Relationships</span></span>
<span data-ttu-id="7df76-130">无</span><span class="sxs-lookup"><span data-stu-id="7df76-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7df76-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7df76-131">JSON Representation</span></span>
<span data-ttu-id="7df76-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7df76-132">Here is a JSON representation of the resource.</span></span>
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




