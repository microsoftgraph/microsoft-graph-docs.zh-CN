---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978569"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="d6eb4-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6eb4-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="d6eb4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6eb4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6eb4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6eb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6eb4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d6eb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6eb4-107">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="d6eb4-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="d6eb4-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6eb4-108">Properties</span></span>
|<span data-ttu-id="d6eb4-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6eb4-109">Property</span></span>|<span data-ttu-id="d6eb4-110">类型</span><span class="sxs-lookup"><span data-stu-id="d6eb4-110">Type</span></span>|<span data-ttu-id="d6eb4-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6eb4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6eb4-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d6eb4-112">hideInstallationProgress</span></span>|<span data-ttu-id="d6eb4-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6eb4-113">Boolean</span></span>|<span data-ttu-id="d6eb4-114">显示或隐藏用户安装进度</span><span class="sxs-lookup"><span data-stu-id="d6eb4-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d6eb4-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="d6eb4-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="d6eb4-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6eb4-116">Boolean</span></span>|<span data-ttu-id="d6eb4-117">允许或阻止用户使用配置文件和应用程序安装完成之前的设备</span><span class="sxs-lookup"><span data-stu-id="d6eb4-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="d6eb4-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d6eb4-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d6eb4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6eb4-119">Boolean</span></span>|<span data-ttu-id="d6eb4-120">允许用户重试上安装失败的设置</span><span class="sxs-lookup"><span data-stu-id="d6eb4-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d6eb4-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d6eb4-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d6eb4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6eb4-122">Boolean</span></span>|<span data-ttu-id="d6eb4-123">允许或阻止上安装失败日志集合</span><span class="sxs-lookup"><span data-stu-id="d6eb4-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d6eb4-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d6eb4-124">customErrorMessage</span></span>|<span data-ttu-id="d6eb4-125">字符串</span><span class="sxs-lookup"><span data-stu-id="d6eb4-125">String</span></span>|<span data-ttu-id="d6eb4-126">设置要在安装失败时显示自定义错误消息</span><span class="sxs-lookup"><span data-stu-id="d6eb4-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d6eb4-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d6eb4-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d6eb4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d6eb4-128">Int32</span></span>|<span data-ttu-id="d6eb4-129">以分钟为单位的设置安装进度超时</span><span class="sxs-lookup"><span data-stu-id="d6eb4-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d6eb4-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d6eb4-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d6eb4-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6eb4-131">Boolean</span></span>|<span data-ttu-id="d6eb4-132">允许用户继续使用设备上安装失败</span><span class="sxs-lookup"><span data-stu-id="d6eb4-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6eb4-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="d6eb4-133">Relationships</span></span>
<span data-ttu-id="d6eb4-134">无</span><span class="sxs-lookup"><span data-stu-id="d6eb4-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6eb4-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6eb4-135">JSON Representation</span></span>
<span data-ttu-id="d6eb4-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6eb4-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





