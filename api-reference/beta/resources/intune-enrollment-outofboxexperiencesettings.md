---
title: outOfBoxExperienceSettings 资源类型
description: 即开体验设置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404601"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="57d97-103">outOfBoxExperienceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="57d97-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="57d97-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="57d97-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57d97-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="57d97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57d97-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57d97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57d97-107">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="57d97-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="57d97-108">属性</span><span class="sxs-lookup"><span data-stu-id="57d97-108">Properties</span></span>
|<span data-ttu-id="57d97-109">属性</span><span class="sxs-lookup"><span data-stu-id="57d97-109">Property</span></span>|<span data-ttu-id="57d97-110">类型</span><span class="sxs-lookup"><span data-stu-id="57d97-110">Type</span></span>|<span data-ttu-id="57d97-111">说明</span><span class="sxs-lookup"><span data-stu-id="57d97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57d97-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="57d97-112">hidePrivacySettings</span></span>|<span data-ttu-id="57d97-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d97-113">Boolean</span></span>|<span data-ttu-id="57d97-114">显示或隐藏给用户的隐私设置</span><span class="sxs-lookup"><span data-stu-id="57d97-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="57d97-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="57d97-115">hideEULA</span></span>|<span data-ttu-id="57d97-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d97-116">Boolean</span></span>|<span data-ttu-id="57d97-117">显示或隐藏 EULA 给用户</span><span class="sxs-lookup"><span data-stu-id="57d97-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="57d97-118">userType</span><span class="sxs-lookup"><span data-stu-id="57d97-118">userType</span></span>|[<span data-ttu-id="57d97-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="57d97-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="57d97-120">用户的类型。</span><span class="sxs-lookup"><span data-stu-id="57d97-120">Type of user.</span></span> <span data-ttu-id="57d97-121">可取值为：`administrator`、`standard`。</span><span class="sxs-lookup"><span data-stu-id="57d97-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="57d97-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="57d97-122">deviceUsageType</span></span>|[<span data-ttu-id="57d97-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="57d97-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="57d97-124">AAD 联接身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="57d97-124">AAD join authentication type.</span></span> <span data-ttu-id="57d97-125">可取值为：`singleUser`、`shared`。</span><span class="sxs-lookup"><span data-stu-id="57d97-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="57d97-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="57d97-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="57d97-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d97-127">Boolean</span></span>|<span data-ttu-id="57d97-128">如果设置，然后跳过键盘选择页面如果语言和区域设置</span><span class="sxs-lookup"><span data-stu-id="57d97-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="57d97-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="57d97-129">hideEscapeLink</span></span>|<span data-ttu-id="57d97-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d97-130">Boolean</span></span>|<span data-ttu-id="57d97-131">如果设置为 true，然后用户无法通过开始与不同的帐户，请在公司登录</span><span class="sxs-lookup"><span data-stu-id="57d97-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="57d97-132">关系</span><span class="sxs-lookup"><span data-stu-id="57d97-132">Relationships</span></span>
<span data-ttu-id="57d97-133">无</span><span class="sxs-lookup"><span data-stu-id="57d97-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57d97-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57d97-134">JSON Representation</span></span>
<span data-ttu-id="57d97-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57d97-135">Here is a JSON representation of the resource.</span></span>
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




