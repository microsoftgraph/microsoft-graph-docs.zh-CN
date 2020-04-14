---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 189751d12f7220dcfa4e3e6985c3913bb7ae0e32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465058"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e3155-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3155-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="e3155-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3155-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3155-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3155-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3155-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3155-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3155-107">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="e3155-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="e3155-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3155-108">Properties</span></span>
|<span data-ttu-id="e3155-109">属性</span><span class="sxs-lookup"><span data-stu-id="e3155-109">Property</span></span>|<span data-ttu-id="e3155-110">类型</span><span class="sxs-lookup"><span data-stu-id="e3155-110">Type</span></span>|<span data-ttu-id="e3155-111">说明</span><span class="sxs-lookup"><span data-stu-id="e3155-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3155-112">inventory</span><span class="sxs-lookup"><span data-stu-id="e3155-112">inventory</span></span>|<span data-ttu-id="e3155-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-113">Boolean</span></span>|<span data-ttu-id="e3155-114">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e3155-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="e3155-115">modernApps</span></span>|<span data-ttu-id="e3155-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-116">Boolean</span></span>|<span data-ttu-id="e3155-117">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e3155-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e3155-118">resourceAccess</span></span>|<span data-ttu-id="e3155-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-119">Boolean</span></span>|<span data-ttu-id="e3155-120">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e3155-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e3155-121">deviceConfiguration</span></span>|<span data-ttu-id="e3155-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-122">Boolean</span></span>|<span data-ttu-id="e3155-123">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e3155-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e3155-124">compliancePolicy</span></span>|<span data-ttu-id="e3155-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-125">Boolean</span></span>|<span data-ttu-id="e3155-126">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e3155-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e3155-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e3155-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3155-128">Boolean</span></span>|<span data-ttu-id="e3155-129">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="e3155-130">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="e3155-130">endpointProtection</span></span>|<span data-ttu-id="e3155-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-131">Boolean</span></span>|<span data-ttu-id="e3155-132">Endpoint Protection 是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="e3155-133">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="e3155-133">officeApps</span></span>|<span data-ttu-id="e3155-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3155-134">Boolean</span></span>|<span data-ttu-id="e3155-135">Office 应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e3155-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3155-136">关系</span><span class="sxs-lookup"><span data-stu-id="e3155-136">Relationships</span></span>
<span data-ttu-id="e3155-137">无</span><span class="sxs-lookup"><span data-stu-id="e3155-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3155-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3155-138">JSON Representation</span></span>
<span data-ttu-id="e3155-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3155-139">Here is a JSON representation of the resource.</span></span>
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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```



