---
title: outOfBoxExperienceSettings 资源类型
description: "\"开箱即用体验\" 设置"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f465297f437f3710f8c789d8683794b7c9d5fa5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773509"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="770ef-103">outOfBoxExperienceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="770ef-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="770ef-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="770ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="770ef-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="770ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="770ef-106">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="770ef-106">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="770ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="770ef-107">Properties</span></span>
|<span data-ttu-id="770ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="770ef-108">Property</span></span>|<span data-ttu-id="770ef-109">类型</span><span class="sxs-lookup"><span data-stu-id="770ef-109">Type</span></span>|<span data-ttu-id="770ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="770ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="770ef-111">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="770ef-111">hidePrivacySettings</span></span>|<span data-ttu-id="770ef-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="770ef-112">Boolean</span></span>|<span data-ttu-id="770ef-113">向用户显示或隐藏隐私设置</span><span class="sxs-lookup"><span data-stu-id="770ef-113">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="770ef-114">hideEULA</span><span class="sxs-lookup"><span data-stu-id="770ef-114">hideEULA</span></span>|<span data-ttu-id="770ef-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="770ef-115">Boolean</span></span>|<span data-ttu-id="770ef-116">向用户显示或隐藏 EULA</span><span class="sxs-lookup"><span data-stu-id="770ef-116">Show or hide EULA to user</span></span>|
|<span data-ttu-id="770ef-117">userType</span><span class="sxs-lookup"><span data-stu-id="770ef-117">userType</span></span>|[<span data-ttu-id="770ef-118">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="770ef-118">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="770ef-119">用户类型。</span><span class="sxs-lookup"><span data-stu-id="770ef-119">Type of user.</span></span> <span data-ttu-id="770ef-120">可取值为：`administrator`、`standard`。</span><span class="sxs-lookup"><span data-stu-id="770ef-120">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="770ef-121">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="770ef-121">deviceUsageType</span></span>|[<span data-ttu-id="770ef-122">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="770ef-122">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="770ef-123">AAD 联接身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="770ef-123">AAD join authentication type.</span></span> <span data-ttu-id="770ef-124">可取值为：`singleUser`、`shared`。</span><span class="sxs-lookup"><span data-stu-id="770ef-124">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="770ef-125">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="770ef-125">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="770ef-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="770ef-126">Boolean</span></span>|<span data-ttu-id="770ef-127">如果设置了语言和区域, 则选择 "设置", 然后跳过 "键盘选择" 页面</span><span class="sxs-lookup"><span data-stu-id="770ef-127">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="770ef-128">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="770ef-128">hideEscapeLink</span></span>|<span data-ttu-id="770ef-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="770ef-129">Boolean</span></span>|<span data-ttu-id="770ef-130">如果设置为 true, 则用户无法在公司登录时使用不同帐户重新开始</span><span class="sxs-lookup"><span data-stu-id="770ef-130">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="770ef-131">关系</span><span class="sxs-lookup"><span data-stu-id="770ef-131">Relationships</span></span>
<span data-ttu-id="770ef-132">无</span><span class="sxs-lookup"><span data-stu-id="770ef-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="770ef-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="770ef-133">JSON Representation</span></span>
<span data-ttu-id="770ef-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="770ef-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```





