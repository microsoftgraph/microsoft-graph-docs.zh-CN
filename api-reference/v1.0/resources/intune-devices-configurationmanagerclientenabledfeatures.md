---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da8a32960b1a8e82f60161e329abcf68916b4f37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451270"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="a45da-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="a45da-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="a45da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a45da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a45da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a45da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a45da-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="a45da-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="a45da-107">属性</span><span class="sxs-lookup"><span data-stu-id="a45da-107">Properties</span></span>
|<span data-ttu-id="a45da-108">属性</span><span class="sxs-lookup"><span data-stu-id="a45da-108">Property</span></span>|<span data-ttu-id="a45da-109">类型</span><span class="sxs-lookup"><span data-stu-id="a45da-109">Type</span></span>|<span data-ttu-id="a45da-110">说明</span><span class="sxs-lookup"><span data-stu-id="a45da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a45da-111">inventory</span><span class="sxs-lookup"><span data-stu-id="a45da-111">inventory</span></span>|<span data-ttu-id="a45da-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-112">Boolean</span></span>|<span data-ttu-id="a45da-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="a45da-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="a45da-114">modernApps</span></span>|<span data-ttu-id="a45da-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-115">Boolean</span></span>|<span data-ttu-id="a45da-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="a45da-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="a45da-117">resourceAccess</span></span>|<span data-ttu-id="a45da-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-118">Boolean</span></span>|<span data-ttu-id="a45da-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="a45da-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a45da-120">deviceConfiguration</span></span>|<span data-ttu-id="a45da-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-121">Boolean</span></span>|<span data-ttu-id="a45da-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="a45da-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a45da-123">compliancePolicy</span></span>|<span data-ttu-id="a45da-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-124">Boolean</span></span>|<span data-ttu-id="a45da-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="a45da-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="a45da-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="a45da-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a45da-127">Boolean</span></span>|<span data-ttu-id="a45da-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="a45da-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="a45da-129">关系</span><span class="sxs-lookup"><span data-stu-id="a45da-129">Relationships</span></span>
<span data-ttu-id="a45da-130">无</span><span class="sxs-lookup"><span data-stu-id="a45da-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a45da-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a45da-131">JSON Representation</span></span>
<span data-ttu-id="a45da-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a45da-132">Here is a JSON representation of the resource.</span></span>
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







