---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d5e167652c57ad7380b7185865dd1437819dbe68
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783338"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="991e7-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="991e7-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="991e7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="991e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="991e7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="991e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="991e7-106">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="991e7-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="991e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="991e7-107">Properties</span></span>
|<span data-ttu-id="991e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="991e7-108">Property</span></span>|<span data-ttu-id="991e7-109">类型</span><span class="sxs-lookup"><span data-stu-id="991e7-109">Type</span></span>|<span data-ttu-id="991e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="991e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="991e7-111">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="991e7-111">hideInstallationProgress</span></span>|<span data-ttu-id="991e7-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="991e7-112">Boolean</span></span>|<span data-ttu-id="991e7-113">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="991e7-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="991e7-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="991e7-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="991e7-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="991e7-115">Boolean</span></span>|<span data-ttu-id="991e7-116">在配置文件和应用安装完成之前允许或阻止用户使用设备</span><span class="sxs-lookup"><span data-stu-id="991e7-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="991e7-117">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="991e7-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="991e7-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="991e7-118">Boolean</span></span>|<span data-ttu-id="991e7-119">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="991e7-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="991e7-120">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="991e7-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="991e7-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="991e7-121">Boolean</span></span>|<span data-ttu-id="991e7-122">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="991e7-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="991e7-123">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="991e7-123">customErrorMessage</span></span>|<span data-ttu-id="991e7-124">String</span><span class="sxs-lookup"><span data-stu-id="991e7-124">String</span></span>|<span data-ttu-id="991e7-125">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="991e7-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="991e7-126">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="991e7-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="991e7-127">Int32</span><span class="sxs-lookup"><span data-stu-id="991e7-127">Int32</span></span>|<span data-ttu-id="991e7-128">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="991e7-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="991e7-129">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="991e7-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="991e7-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="991e7-130">Boolean</span></span>|<span data-ttu-id="991e7-131">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="991e7-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="991e7-132">关系</span><span class="sxs-lookup"><span data-stu-id="991e7-132">Relationships</span></span>
<span data-ttu-id="991e7-133">无</span><span class="sxs-lookup"><span data-stu-id="991e7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="991e7-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="991e7-134">JSON Representation</span></span>
<span data-ttu-id="991e7-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="991e7-135">Here is a JSON representation of the resource.</span></span>
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



