---
title: outOfBoxExperienceSettings 资源类型
description: "\"开箱即用体验\" 设置"
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82bfd9a7126298958d35ad121b22115bb1f71241
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460705"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="d336c-103">outOfBoxExperienceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d336c-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="d336c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d336c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d336c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d336c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d336c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d336c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d336c-107">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="d336c-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="d336c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d336c-108">Properties</span></span>
|<span data-ttu-id="d336c-109">属性</span><span class="sxs-lookup"><span data-stu-id="d336c-109">Property</span></span>|<span data-ttu-id="d336c-110">类型</span><span class="sxs-lookup"><span data-stu-id="d336c-110">Type</span></span>|<span data-ttu-id="d336c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d336c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d336c-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="d336c-112">hidePrivacySettings</span></span>|<span data-ttu-id="d336c-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="d336c-113">Boolean</span></span>|<span data-ttu-id="d336c-114">向用户显示或隐藏隐私设置</span><span class="sxs-lookup"><span data-stu-id="d336c-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="d336c-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="d336c-115">hideEULA</span></span>|<span data-ttu-id="d336c-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="d336c-116">Boolean</span></span>|<span data-ttu-id="d336c-117">向用户显示或隐藏 EULA</span><span class="sxs-lookup"><span data-stu-id="d336c-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="d336c-118">userType</span><span class="sxs-lookup"><span data-stu-id="d336c-118">userType</span></span>|[<span data-ttu-id="d336c-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="d336c-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="d336c-120">用户类型。</span><span class="sxs-lookup"><span data-stu-id="d336c-120">Type of user.</span></span> <span data-ttu-id="d336c-121">可取值为：`administrator`、`standard`。</span><span class="sxs-lookup"><span data-stu-id="d336c-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="d336c-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="d336c-122">deviceUsageType</span></span>|[<span data-ttu-id="d336c-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="d336c-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="d336c-124">AAD 联接身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="d336c-124">AAD join authentication type.</span></span> <span data-ttu-id="d336c-125">可取值为：`singleUser`、`shared`。</span><span class="sxs-lookup"><span data-stu-id="d336c-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="d336c-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="d336c-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="d336c-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="d336c-127">Boolean</span></span>|<span data-ttu-id="d336c-128">如果设置了语言和区域，则选择 "设置"，然后跳过 "键盘选择" 页面</span><span class="sxs-lookup"><span data-stu-id="d336c-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="d336c-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="d336c-129">hideEscapeLink</span></span>|<span data-ttu-id="d336c-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="d336c-130">Boolean</span></span>|<span data-ttu-id="d336c-131">如果设置为 true，则用户无法在公司登录时使用不同帐户重新开始</span><span class="sxs-lookup"><span data-stu-id="d336c-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="d336c-132">关系</span><span class="sxs-lookup"><span data-stu-id="d336c-132">Relationships</span></span>
<span data-ttu-id="d336c-133">无</span><span class="sxs-lookup"><span data-stu-id="d336c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d336c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d336c-134">JSON Representation</span></span>
<span data-ttu-id="d336c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d336c-135">Here is a JSON representation of the resource.</span></span>
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



