---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9407e1d035a5cd50db7b071f562acb4eb2d007b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371983"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="83c80-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="83c80-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="83c80-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83c80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83c80-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83c80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83c80-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="83c80-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="83c80-107">属性</span><span class="sxs-lookup"><span data-stu-id="83c80-107">Properties</span></span>
|<span data-ttu-id="83c80-108">属性</span><span class="sxs-lookup"><span data-stu-id="83c80-108">Property</span></span>|<span data-ttu-id="83c80-109">类型</span><span class="sxs-lookup"><span data-stu-id="83c80-109">Type</span></span>|<span data-ttu-id="83c80-110">说明</span><span class="sxs-lookup"><span data-stu-id="83c80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c80-111">inventory</span><span class="sxs-lookup"><span data-stu-id="83c80-111">inventory</span></span>|<span data-ttu-id="83c80-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-112">Boolean</span></span>|<span data-ttu-id="83c80-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="83c80-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="83c80-114">modernApps</span></span>|<span data-ttu-id="83c80-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-115">Boolean</span></span>|<span data-ttu-id="83c80-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="83c80-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="83c80-117">resourceAccess</span></span>|<span data-ttu-id="83c80-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-118">Boolean</span></span>|<span data-ttu-id="83c80-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="83c80-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="83c80-120">deviceConfiguration</span></span>|<span data-ttu-id="83c80-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-121">Boolean</span></span>|<span data-ttu-id="83c80-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="83c80-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="83c80-123">compliancePolicy</span></span>|<span data-ttu-id="83c80-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-124">Boolean</span></span>|<span data-ttu-id="83c80-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="83c80-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="83c80-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="83c80-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-127">Boolean</span></span>|<span data-ttu-id="83c80-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="83c80-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="83c80-129">endpointProtection</span></span>|<span data-ttu-id="83c80-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-130">Boolean</span></span>|<span data-ttu-id="83c80-131">Endpoint Protection 是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="83c80-132">Officeoffice</span><span class="sxs-lookup"><span data-stu-id="83c80-132">officeApps</span></span>|<span data-ttu-id="83c80-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="83c80-133">Boolean</span></span>|<span data-ttu-id="83c80-134">Office 应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="83c80-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="83c80-135">关系</span><span class="sxs-lookup"><span data-stu-id="83c80-135">Relationships</span></span>
<span data-ttu-id="83c80-136">无</span><span class="sxs-lookup"><span data-stu-id="83c80-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83c80-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83c80-137">JSON Representation</span></span>
<span data-ttu-id="83c80-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83c80-138">Here is a JSON representation of the resource.</span></span>
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



