---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c69e0ae9528a31ec7512348931e9a6eb0b1dd7b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838939"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="0895e-103">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="0895e-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="0895e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0895e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0895e-105">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="0895e-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="0895e-106">属性</span><span class="sxs-lookup"><span data-stu-id="0895e-106">Properties</span></span>
|<span data-ttu-id="0895e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0895e-107">Property</span></span>|<span data-ttu-id="0895e-108">类型</span><span class="sxs-lookup"><span data-stu-id="0895e-108">Type</span></span>|<span data-ttu-id="0895e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0895e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0895e-110">inventory</span><span class="sxs-lookup"><span data-stu-id="0895e-110">inventory</span></span>|<span data-ttu-id="0895e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-111">Boolean</span></span>|<span data-ttu-id="0895e-112">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="0895e-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="0895e-113">modernApps</span></span>|<span data-ttu-id="0895e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-114">Boolean</span></span>|<span data-ttu-id="0895e-115">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="0895e-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0895e-116">resourceAccess</span></span>|<span data-ttu-id="0895e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-117">Boolean</span></span>|<span data-ttu-id="0895e-118">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="0895e-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0895e-119">deviceConfiguration</span></span>|<span data-ttu-id="0895e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-120">Boolean</span></span>|<span data-ttu-id="0895e-121">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="0895e-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0895e-122">compliancePolicy</span></span>|<span data-ttu-id="0895e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-123">Boolean</span></span>|<span data-ttu-id="0895e-124">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="0895e-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="0895e-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="0895e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="0895e-126">Boolean</span></span>|<span data-ttu-id="0895e-127">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="0895e-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0895e-128">关系</span><span class="sxs-lookup"><span data-stu-id="0895e-128">Relationships</span></span>
<span data-ttu-id="0895e-129">无</span><span class="sxs-lookup"><span data-stu-id="0895e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0895e-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0895e-130">JSON Representation</span></span>
<span data-ttu-id="0895e-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0895e-131">Here is a JSON representation of the resource.</span></span>
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



