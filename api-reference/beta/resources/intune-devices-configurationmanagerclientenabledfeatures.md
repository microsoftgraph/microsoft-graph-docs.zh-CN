---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2909c1cbc7fd65ff71c36fe777fd8bcbce9749cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968566"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="8c7a5-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c7a5-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="8c7a5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c7a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c7a5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c7a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c7a5-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="8c7a5-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="8c7a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c7a5-107">Properties</span></span>
|<span data-ttu-id="8c7a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c7a5-108">Property</span></span>|<span data-ttu-id="8c7a5-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c7a5-109">Type</span></span>|<span data-ttu-id="8c7a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c7a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c7a5-111">inventory</span><span class="sxs-lookup"><span data-stu-id="8c7a5-111">inventory</span></span>|<span data-ttu-id="8c7a5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-112">Boolean</span></span>|<span data-ttu-id="8c7a5-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="8c7a5-114">modernApps</span></span>|<span data-ttu-id="8c7a5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-115">Boolean</span></span>|<span data-ttu-id="8c7a5-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="8c7a5-117">resourceAccess</span></span>|<span data-ttu-id="8c7a5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-118">Boolean</span></span>|<span data-ttu-id="8c7a5-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c7a5-120">deviceConfiguration</span></span>|<span data-ttu-id="8c7a5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-121">Boolean</span></span>|<span data-ttu-id="8c7a5-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8c7a5-123">compliancePolicy</span></span>|<span data-ttu-id="8c7a5-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-124">Boolean</span></span>|<span data-ttu-id="8c7a5-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="8c7a5-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="8c7a5-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-127">Boolean</span></span>|<span data-ttu-id="8c7a5-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="8c7a5-129">endpointProtection</span></span>|<span data-ttu-id="8c7a5-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-130">Boolean</span></span>|<span data-ttu-id="8c7a5-131">Endpoint Protection 是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="8c7a5-132">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="8c7a5-132">officeApps</span></span>|<span data-ttu-id="8c7a5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c7a5-133">Boolean</span></span>|<span data-ttu-id="8c7a5-134">Office 应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="8c7a5-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c7a5-135">关系</span><span class="sxs-lookup"><span data-stu-id="8c7a5-135">Relationships</span></span>
<span data-ttu-id="8c7a5-136">无</span><span class="sxs-lookup"><span data-stu-id="8c7a5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c7a5-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c7a5-137">JSON Representation</span></span>
<span data-ttu-id="8c7a5-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c7a5-138">Here is a JSON representation of the resource.</span></span>
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





