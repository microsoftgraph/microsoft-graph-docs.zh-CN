---
title: outOfBoxExperienceSettings 资源类型
description: 即开体验设置
ms.openlocfilehash: 7d685c7e229828309e2ee759396215c3cd8dfac9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048864"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="7409f-103">outOfBoxExperienceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7409f-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="7409f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7409f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7409f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7409f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7409f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7409f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7409f-107">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="7409f-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="7409f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7409f-108">Properties</span></span>
|<span data-ttu-id="7409f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7409f-109">Property</span></span>|<span data-ttu-id="7409f-110">类型</span><span class="sxs-lookup"><span data-stu-id="7409f-110">Type</span></span>|<span data-ttu-id="7409f-111">说明</span><span class="sxs-lookup"><span data-stu-id="7409f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7409f-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="7409f-112">hidePrivacySettings</span></span>|<span data-ttu-id="7409f-113">布尔</span><span class="sxs-lookup"><span data-stu-id="7409f-113">Boolean</span></span>|<span data-ttu-id="7409f-114">显示或隐藏给用户的隐私设置</span><span class="sxs-lookup"><span data-stu-id="7409f-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="7409f-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="7409f-115">hideEULA</span></span>|<span data-ttu-id="7409f-116">布尔</span><span class="sxs-lookup"><span data-stu-id="7409f-116">Boolean</span></span>|<span data-ttu-id="7409f-117">显示或隐藏 EULA 给用户</span><span class="sxs-lookup"><span data-stu-id="7409f-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="7409f-118">userType</span><span class="sxs-lookup"><span data-stu-id="7409f-118">userType</span></span>|[<span data-ttu-id="7409f-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="7409f-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="7409f-120">用户的类型。</span><span class="sxs-lookup"><span data-stu-id="7409f-120">Type of user.</span></span> <span data-ttu-id="7409f-121">可取值为：`administrator`、`standard`。</span><span class="sxs-lookup"><span data-stu-id="7409f-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="7409f-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="7409f-122">deviceUsageType</span></span>|[<span data-ttu-id="7409f-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="7409f-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="7409f-124">AAD 联接身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="7409f-124">AAD join authentication type.</span></span> <span data-ttu-id="7409f-125">可取值为：`singleUser`、`shared`。</span><span class="sxs-lookup"><span data-stu-id="7409f-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="7409f-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="7409f-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="7409f-127">布尔</span><span class="sxs-lookup"><span data-stu-id="7409f-127">Boolean</span></span>|<span data-ttu-id="7409f-128">如果设置，然后跳过键盘选择页面如果语言和区域设置</span><span class="sxs-lookup"><span data-stu-id="7409f-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="7409f-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="7409f-129">hideEscapeLink</span></span>|<span data-ttu-id="7409f-130">布尔</span><span class="sxs-lookup"><span data-stu-id="7409f-130">Boolean</span></span>|<span data-ttu-id="7409f-131">如果设置为 true，然后用户无法通过开始与不同的帐户，请在公司登录</span><span class="sxs-lookup"><span data-stu-id="7409f-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="7409f-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="7409f-132">Relationships</span></span>
<span data-ttu-id="7409f-133">无</span><span class="sxs-lookup"><span data-stu-id="7409f-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7409f-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7409f-134">JSON Representation</span></span>
<span data-ttu-id="7409f-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7409f-135">Here is a JSON representation of the resource.</span></span>
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





