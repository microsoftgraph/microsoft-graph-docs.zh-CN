---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfae041f1aab4c4ea74490d372350c5c0c2087b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528684"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="a53bd-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="a53bd-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="a53bd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a53bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a53bd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a53bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a53bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a53bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a53bd-107">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="a53bd-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="a53bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="a53bd-108">Properties</span></span>
|<span data-ttu-id="a53bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="a53bd-109">Property</span></span>|<span data-ttu-id="a53bd-110">类型</span><span class="sxs-lookup"><span data-stu-id="a53bd-110">Type</span></span>|<span data-ttu-id="a53bd-111">说明</span><span class="sxs-lookup"><span data-stu-id="a53bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a53bd-112">inventory</span><span class="sxs-lookup"><span data-stu-id="a53bd-112">inventory</span></span>|<span data-ttu-id="a53bd-113">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-113">Boolean</span></span>|<span data-ttu-id="a53bd-114">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="a53bd-115">modernApps</span></span>|<span data-ttu-id="a53bd-116">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-116">Boolean</span></span>|<span data-ttu-id="a53bd-117">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="a53bd-118">resourceAccess</span></span>|<span data-ttu-id="a53bd-119">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-119">Boolean</span></span>|<span data-ttu-id="a53bd-120">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a53bd-121">deviceConfiguration</span></span>|<span data-ttu-id="a53bd-122">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-122">Boolean</span></span>|<span data-ttu-id="a53bd-123">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a53bd-124">compliancePolicy</span></span>|<span data-ttu-id="a53bd-125">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-125">Boolean</span></span>|<span data-ttu-id="a53bd-126">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="a53bd-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="a53bd-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a53bd-128">Boolean</span></span>|<span data-ttu-id="a53bd-129">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-130">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="a53bd-130">endpointProtection</span></span>|<span data-ttu-id="a53bd-131">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-131">Boolean</span></span>|<span data-ttu-id="a53bd-132">Endpoint Protection 是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="a53bd-133">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="a53bd-133">officeApps</span></span>|<span data-ttu-id="a53bd-134">布尔</span><span class="sxs-lookup"><span data-stu-id="a53bd-134">Boolean</span></span>|<span data-ttu-id="a53bd-135">Office 应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a53bd-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="a53bd-136">关系</span><span class="sxs-lookup"><span data-stu-id="a53bd-136">Relationships</span></span>
<span data-ttu-id="a53bd-137">无</span><span class="sxs-lookup"><span data-stu-id="a53bd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a53bd-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a53bd-138">JSON Representation</span></span>
<span data-ttu-id="a53bd-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a53bd-139">Here is a JSON representation of the resource.</span></span>
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



