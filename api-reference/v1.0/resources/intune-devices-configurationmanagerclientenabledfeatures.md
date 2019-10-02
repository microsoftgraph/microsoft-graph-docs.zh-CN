---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c68fa195584c8d30cbe6a9b942a453b4f6a9218
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357036"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="137ac-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="137ac-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="137ac-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="137ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="137ac-105">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="137ac-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="137ac-106">属性</span><span class="sxs-lookup"><span data-stu-id="137ac-106">Properties</span></span>
|<span data-ttu-id="137ac-107">属性</span><span class="sxs-lookup"><span data-stu-id="137ac-107">Property</span></span>|<span data-ttu-id="137ac-108">类型</span><span class="sxs-lookup"><span data-stu-id="137ac-108">Type</span></span>|<span data-ttu-id="137ac-109">说明</span><span class="sxs-lookup"><span data-stu-id="137ac-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="137ac-110">inventory</span><span class="sxs-lookup"><span data-stu-id="137ac-110">inventory</span></span>|<span data-ttu-id="137ac-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-111">Boolean</span></span>|<span data-ttu-id="137ac-112">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="137ac-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="137ac-113">modernApps</span></span>|<span data-ttu-id="137ac-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-114">Boolean</span></span>|<span data-ttu-id="137ac-115">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="137ac-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="137ac-116">resourceAccess</span></span>|<span data-ttu-id="137ac-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-117">Boolean</span></span>|<span data-ttu-id="137ac-118">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="137ac-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="137ac-119">deviceConfiguration</span></span>|<span data-ttu-id="137ac-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-120">Boolean</span></span>|<span data-ttu-id="137ac-121">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="137ac-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="137ac-122">compliancePolicy</span></span>|<span data-ttu-id="137ac-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-123">Boolean</span></span>|<span data-ttu-id="137ac-124">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="137ac-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="137ac-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="137ac-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="137ac-126">Boolean</span></span>|<span data-ttu-id="137ac-127">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="137ac-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="137ac-128">关系</span><span class="sxs-lookup"><span data-stu-id="137ac-128">Relationships</span></span>
<span data-ttu-id="137ac-129">无</span><span class="sxs-lookup"><span data-stu-id="137ac-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="137ac-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="137ac-130">JSON Representation</span></span>
<span data-ttu-id="137ac-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="137ac-131">Here is a JSON representation of the resource.</span></span>
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




