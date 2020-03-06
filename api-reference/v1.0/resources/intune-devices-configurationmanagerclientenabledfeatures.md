---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e8622f6f1772948295f9389cf97aef0b6f260e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533312"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="fc5bf-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc5bf-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="fc5bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc5bf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc5bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc5bf-106">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="fc5bf-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="fc5bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc5bf-107">Properties</span></span>
|<span data-ttu-id="fc5bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc5bf-108">Property</span></span>|<span data-ttu-id="fc5bf-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc5bf-109">Type</span></span>|<span data-ttu-id="fc5bf-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc5bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc5bf-111">inventory</span><span class="sxs-lookup"><span data-stu-id="fc5bf-111">inventory</span></span>|<span data-ttu-id="fc5bf-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-112">Boolean</span></span>|<span data-ttu-id="fc5bf-113">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="fc5bf-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="fc5bf-114">modernApps</span></span>|<span data-ttu-id="fc5bf-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-115">Boolean</span></span>|<span data-ttu-id="fc5bf-116">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="fc5bf-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="fc5bf-117">resourceAccess</span></span>|<span data-ttu-id="fc5bf-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-118">Boolean</span></span>|<span data-ttu-id="fc5bf-119">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="fc5bf-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc5bf-120">deviceConfiguration</span></span>|<span data-ttu-id="fc5bf-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-121">Boolean</span></span>|<span data-ttu-id="fc5bf-122">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="fc5bf-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fc5bf-123">compliancePolicy</span></span>|<span data-ttu-id="fc5bf-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-124">Boolean</span></span>|<span data-ttu-id="fc5bf-125">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="fc5bf-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="fc5bf-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="fc5bf-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5bf-127">Boolean</span></span>|<span data-ttu-id="fc5bf-128">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="fc5bf-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc5bf-129">关系</span><span class="sxs-lookup"><span data-stu-id="fc5bf-129">Relationships</span></span>
<span data-ttu-id="fc5bf-130">无</span><span class="sxs-lookup"><span data-stu-id="fc5bf-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc5bf-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc5bf-131">JSON Representation</span></span>
<span data-ttu-id="fc5bf-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc5bf-132">Here is a JSON representation of the resource.</span></span>
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




