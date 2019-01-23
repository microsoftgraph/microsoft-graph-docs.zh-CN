---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399932"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="9ca06-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ca06-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="9ca06-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9ca06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ca06-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ca06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ca06-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ca06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ca06-107">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="9ca06-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="9ca06-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ca06-108">Properties</span></span>
|<span data-ttu-id="9ca06-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ca06-109">Property</span></span>|<span data-ttu-id="9ca06-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ca06-110">Type</span></span>|<span data-ttu-id="9ca06-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ca06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ca06-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="9ca06-112">hideInstallationProgress</span></span>|<span data-ttu-id="9ca06-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca06-113">Boolean</span></span>|<span data-ttu-id="9ca06-114">显示或隐藏用户安装进度</span><span class="sxs-lookup"><span data-stu-id="9ca06-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="9ca06-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="9ca06-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="9ca06-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca06-116">Boolean</span></span>|<span data-ttu-id="9ca06-117">允许或阻止用户使用配置文件和应用程序安装完成之前的设备</span><span class="sxs-lookup"><span data-stu-id="9ca06-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="9ca06-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="9ca06-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="9ca06-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca06-119">Boolean</span></span>|<span data-ttu-id="9ca06-120">允许用户重试上安装失败的设置</span><span class="sxs-lookup"><span data-stu-id="9ca06-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="9ca06-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="9ca06-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="9ca06-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca06-122">Boolean</span></span>|<span data-ttu-id="9ca06-123">允许或阻止上安装失败日志集合</span><span class="sxs-lookup"><span data-stu-id="9ca06-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="9ca06-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="9ca06-124">customErrorMessage</span></span>|<span data-ttu-id="9ca06-125">String</span><span class="sxs-lookup"><span data-stu-id="9ca06-125">String</span></span>|<span data-ttu-id="9ca06-126">设置要在安装失败时显示自定义错误消息</span><span class="sxs-lookup"><span data-stu-id="9ca06-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="9ca06-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="9ca06-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="9ca06-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9ca06-128">Int32</span></span>|<span data-ttu-id="9ca06-129">以分钟为单位的设置安装进度超时</span><span class="sxs-lookup"><span data-stu-id="9ca06-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="9ca06-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="9ca06-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="9ca06-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca06-131">Boolean</span></span>|<span data-ttu-id="9ca06-132">允许用户继续使用设备上安装失败</span><span class="sxs-lookup"><span data-stu-id="9ca06-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ca06-133">关系</span><span class="sxs-lookup"><span data-stu-id="9ca06-133">Relationships</span></span>
<span data-ttu-id="9ca06-134">无</span><span class="sxs-lookup"><span data-stu-id="9ca06-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ca06-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ca06-135">JSON Representation</span></span>
<span data-ttu-id="9ca06-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ca06-136">Here is a JSON representation of the resource.</span></span>
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




