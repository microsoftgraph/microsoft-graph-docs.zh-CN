---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425902"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="85a9e-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="85a9e-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="85a9e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="85a9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85a9e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85a9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85a9e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85a9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85a9e-107">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="85a9e-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="85a9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="85a9e-108">Properties</span></span>
|<span data-ttu-id="85a9e-109">属性</span><span class="sxs-lookup"><span data-stu-id="85a9e-109">Property</span></span>|<span data-ttu-id="85a9e-110">类型</span><span class="sxs-lookup"><span data-stu-id="85a9e-110">Type</span></span>|<span data-ttu-id="85a9e-111">说明</span><span class="sxs-lookup"><span data-stu-id="85a9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85a9e-112">inventory</span><span class="sxs-lookup"><span data-stu-id="85a9e-112">inventory</span></span>|<span data-ttu-id="85a9e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-113">Boolean</span></span>|<span data-ttu-id="85a9e-114">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="85a9e-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="85a9e-115">modernApps</span></span>|<span data-ttu-id="85a9e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-116">Boolean</span></span>|<span data-ttu-id="85a9e-117">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="85a9e-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="85a9e-118">resourceAccess</span></span>|<span data-ttu-id="85a9e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-119">Boolean</span></span>|<span data-ttu-id="85a9e-120">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="85a9e-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="85a9e-121">deviceConfiguration</span></span>|<span data-ttu-id="85a9e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-122">Boolean</span></span>|<span data-ttu-id="85a9e-123">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="85a9e-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="85a9e-124">compliancePolicy</span></span>|<span data-ttu-id="85a9e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-125">Boolean</span></span>|<span data-ttu-id="85a9e-126">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="85a9e-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="85a9e-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="85a9e-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="85a9e-128">Boolean</span></span>|<span data-ttu-id="85a9e-129">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="85a9e-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="85a9e-130">关系</span><span class="sxs-lookup"><span data-stu-id="85a9e-130">Relationships</span></span>
<span data-ttu-id="85a9e-131">无</span><span class="sxs-lookup"><span data-stu-id="85a9e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85a9e-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85a9e-132">JSON Representation</span></span>
<span data-ttu-id="85a9e-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85a9e-133">Here is a JSON representation of the resource.</span></span>
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




