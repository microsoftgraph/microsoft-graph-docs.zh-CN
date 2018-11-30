---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
ms.openlocfilehash: 54d5d40a50b2946fec1c69c619dc76bec1f32502
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010424"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="3d631-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d631-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="3d631-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3d631-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d631-105">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="3d631-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="3d631-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d631-106">Properties</span></span>
|<span data-ttu-id="3d631-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d631-107">Property</span></span>|<span data-ttu-id="3d631-108">类型</span><span class="sxs-lookup"><span data-stu-id="3d631-108">Type</span></span>|<span data-ttu-id="3d631-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d631-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d631-110">inventory</span><span class="sxs-lookup"><span data-stu-id="3d631-110">inventory</span></span>|<span data-ttu-id="3d631-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-111">Boolean</span></span>|<span data-ttu-id="3d631-112">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="3d631-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="3d631-113">modernApps</span></span>|<span data-ttu-id="3d631-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-114">Boolean</span></span>|<span data-ttu-id="3d631-115">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="3d631-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="3d631-116">resourceAccess</span></span>|<span data-ttu-id="3d631-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-117">Boolean</span></span>|<span data-ttu-id="3d631-118">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="3d631-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d631-119">deviceConfiguration</span></span>|<span data-ttu-id="3d631-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-120">Boolean</span></span>|<span data-ttu-id="3d631-121">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="3d631-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3d631-122">compliancePolicy</span></span>|<span data-ttu-id="3d631-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-123">Boolean</span></span>|<span data-ttu-id="3d631-124">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="3d631-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="3d631-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="3d631-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d631-126">Boolean</span></span>|<span data-ttu-id="3d631-127">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="3d631-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d631-128">关系</span><span class="sxs-lookup"><span data-stu-id="3d631-128">Relationships</span></span>
<span data-ttu-id="3d631-129">无</span><span class="sxs-lookup"><span data-stu-id="3d631-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d631-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d631-130">JSON Representation</span></span>
<span data-ttu-id="3d631-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d631-131">Here is a JSON representation of the resource.</span></span>
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



