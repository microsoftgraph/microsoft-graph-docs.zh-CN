---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684a447b82f285784eda1bf71c13f35d766a570
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148683"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="32576-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="32576-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="32576-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32576-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32576-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32576-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32576-106">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="32576-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="32576-107">属性</span><span class="sxs-lookup"><span data-stu-id="32576-107">Properties</span></span>
|<span data-ttu-id="32576-108">属性</span><span class="sxs-lookup"><span data-stu-id="32576-108">Property</span></span>|<span data-ttu-id="32576-109">类型</span><span class="sxs-lookup"><span data-stu-id="32576-109">Type</span></span>|<span data-ttu-id="32576-110">说明</span><span class="sxs-lookup"><span data-stu-id="32576-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32576-111">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="32576-111">hideInstallationProgress</span></span>|<span data-ttu-id="32576-112">布尔</span><span class="sxs-lookup"><span data-stu-id="32576-112">Boolean</span></span>|<span data-ttu-id="32576-113">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="32576-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="32576-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="32576-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="32576-115">布尔</span><span class="sxs-lookup"><span data-stu-id="32576-115">Boolean</span></span>|<span data-ttu-id="32576-116">在配置文件和应用安装完成之前允许或阻止用户使用设备</span><span class="sxs-lookup"><span data-stu-id="32576-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="32576-117">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="32576-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="32576-118">布尔</span><span class="sxs-lookup"><span data-stu-id="32576-118">Boolean</span></span>|<span data-ttu-id="32576-119">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="32576-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="32576-120">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="32576-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="32576-121">布尔</span><span class="sxs-lookup"><span data-stu-id="32576-121">Boolean</span></span>|<span data-ttu-id="32576-122">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="32576-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="32576-123">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="32576-123">customErrorMessage</span></span>|<span data-ttu-id="32576-124">字符串</span><span class="sxs-lookup"><span data-stu-id="32576-124">String</span></span>|<span data-ttu-id="32576-125">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="32576-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="32576-126">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="32576-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="32576-127">Int32</span><span class="sxs-lookup"><span data-stu-id="32576-127">Int32</span></span>|<span data-ttu-id="32576-128">设置安装进度超时 (分钟)</span><span class="sxs-lookup"><span data-stu-id="32576-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="32576-129">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="32576-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="32576-130">布尔</span><span class="sxs-lookup"><span data-stu-id="32576-130">Boolean</span></span>|<span data-ttu-id="32576-131">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="32576-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="32576-132">关系</span><span class="sxs-lookup"><span data-stu-id="32576-132">Relationships</span></span>
<span data-ttu-id="32576-133">无</span><span class="sxs-lookup"><span data-stu-id="32576-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32576-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32576-134">JSON Representation</span></span>
<span data-ttu-id="32576-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32576-135">Here is a JSON representation of the resource.</span></span>
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




