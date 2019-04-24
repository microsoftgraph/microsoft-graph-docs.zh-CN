---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467307"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="2b79b-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b79b-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="2b79b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b79b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b79b-105">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="2b79b-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="2b79b-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b79b-106">Properties</span></span>
|<span data-ttu-id="2b79b-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b79b-107">Property</span></span>|<span data-ttu-id="2b79b-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b79b-108">Type</span></span>|<span data-ttu-id="2b79b-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b79b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b79b-110">inventory</span><span class="sxs-lookup"><span data-stu-id="2b79b-110">inventory</span></span>|<span data-ttu-id="2b79b-111">布尔</span><span class="sxs-lookup"><span data-stu-id="2b79b-111">Boolean</span></span>|<span data-ttu-id="2b79b-112">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="2b79b-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="2b79b-113">modernApps</span></span>|<span data-ttu-id="2b79b-114">布尔</span><span class="sxs-lookup"><span data-stu-id="2b79b-114">Boolean</span></span>|<span data-ttu-id="2b79b-115">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="2b79b-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="2b79b-116">resourceAccess</span></span>|<span data-ttu-id="2b79b-117">布尔</span><span class="sxs-lookup"><span data-stu-id="2b79b-117">Boolean</span></span>|<span data-ttu-id="2b79b-118">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="2b79b-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b79b-119">deviceConfiguration</span></span>|<span data-ttu-id="2b79b-120">布尔</span><span class="sxs-lookup"><span data-stu-id="2b79b-120">Boolean</span></span>|<span data-ttu-id="2b79b-121">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="2b79b-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2b79b-122">compliancePolicy</span></span>|<span data-ttu-id="2b79b-123">布尔</span><span class="sxs-lookup"><span data-stu-id="2b79b-123">Boolean</span></span>|<span data-ttu-id="2b79b-124">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="2b79b-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="2b79b-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="2b79b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b79b-126">Boolean</span></span>|<span data-ttu-id="2b79b-127">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="2b79b-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b79b-128">关系</span><span class="sxs-lookup"><span data-stu-id="2b79b-128">Relationships</span></span>
<span data-ttu-id="2b79b-129">无</span><span class="sxs-lookup"><span data-stu-id="2b79b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b79b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b79b-130">JSON Representation</span></span>
<span data-ttu-id="2b79b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b79b-131">Here is a JSON representation of the resource.</span></span>
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



