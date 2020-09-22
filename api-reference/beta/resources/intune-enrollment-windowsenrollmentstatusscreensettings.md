---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 645216f83bee04008fd39d48c963e43025adc8a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031541"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="d98c6-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d98c6-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="d98c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d98c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d98c6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d98c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d98c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98c6-107">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="d98c6-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="d98c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d98c6-108">Properties</span></span>
|<span data-ttu-id="d98c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="d98c6-109">Property</span></span>|<span data-ttu-id="d98c6-110">类型</span><span class="sxs-lookup"><span data-stu-id="d98c6-110">Type</span></span>|<span data-ttu-id="d98c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="d98c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98c6-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d98c6-112">hideInstallationProgress</span></span>|<span data-ttu-id="d98c6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c6-113">Boolean</span></span>|<span data-ttu-id="d98c6-114">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="d98c6-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d98c6-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="d98c6-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="d98c6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c6-116">Boolean</span></span>|<span data-ttu-id="d98c6-117">在配置文件和应用安装完成之前允许或阻止用户使用设备</span><span class="sxs-lookup"><span data-stu-id="d98c6-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="d98c6-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d98c6-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d98c6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c6-119">Boolean</span></span>|<span data-ttu-id="d98c6-120">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="d98c6-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d98c6-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d98c6-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d98c6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c6-122">Boolean</span></span>|<span data-ttu-id="d98c6-123">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="d98c6-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d98c6-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d98c6-124">customErrorMessage</span></span>|<span data-ttu-id="d98c6-125">String</span><span class="sxs-lookup"><span data-stu-id="d98c6-125">String</span></span>|<span data-ttu-id="d98c6-126">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="d98c6-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d98c6-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d98c6-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d98c6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d98c6-128">Int32</span></span>|<span data-ttu-id="d98c6-129">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="d98c6-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d98c6-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d98c6-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d98c6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98c6-131">Boolean</span></span>|<span data-ttu-id="d98c6-132">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="d98c6-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="d98c6-133">关系</span><span class="sxs-lookup"><span data-stu-id="d98c6-133">Relationships</span></span>
<span data-ttu-id="d98c6-134">无</span><span class="sxs-lookup"><span data-stu-id="d98c6-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d98c6-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d98c6-135">JSON Representation</span></span>
<span data-ttu-id="d98c6-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d98c6-136">Here is a JSON representation of the resource.</span></span>
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






