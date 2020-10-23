---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 722f262688a35f6e14ae495f0e5cf5ee5976beb5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697509"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="6586d-103">windowsEnrollmentStatusScreenSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6586d-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="6586d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6586d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6586d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6586d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6586d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6586d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6586d-107">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="6586d-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="6586d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6586d-108">Properties</span></span>
|<span data-ttu-id="6586d-109">属性</span><span class="sxs-lookup"><span data-stu-id="6586d-109">Property</span></span>|<span data-ttu-id="6586d-110">类型</span><span class="sxs-lookup"><span data-stu-id="6586d-110">Type</span></span>|<span data-ttu-id="6586d-111">说明</span><span class="sxs-lookup"><span data-stu-id="6586d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6586d-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="6586d-112">hideInstallationProgress</span></span>|<span data-ttu-id="6586d-113">布尔</span><span class="sxs-lookup"><span data-stu-id="6586d-113">Boolean</span></span>|<span data-ttu-id="6586d-114">显示或隐藏用户的安装进度</span><span class="sxs-lookup"><span data-stu-id="6586d-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="6586d-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="6586d-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="6586d-116">布尔</span><span class="sxs-lookup"><span data-stu-id="6586d-116">Boolean</span></span>|<span data-ttu-id="6586d-117">在配置文件和应用安装完成之前允许或阻止用户使用设备</span><span class="sxs-lookup"><span data-stu-id="6586d-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="6586d-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="6586d-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="6586d-119">布尔</span><span class="sxs-lookup"><span data-stu-id="6586d-119">Boolean</span></span>|<span data-ttu-id="6586d-120">允许用户在安装失败时重试安装程序</span><span class="sxs-lookup"><span data-stu-id="6586d-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="6586d-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="6586d-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="6586d-122">布尔</span><span class="sxs-lookup"><span data-stu-id="6586d-122">Boolean</span></span>|<span data-ttu-id="6586d-123">在安装失败时允许或阻止日志集合</span><span class="sxs-lookup"><span data-stu-id="6586d-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="6586d-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="6586d-124">customErrorMessage</span></span>|<span data-ttu-id="6586d-125">String</span><span class="sxs-lookup"><span data-stu-id="6586d-125">String</span></span>|<span data-ttu-id="6586d-126">设置自定义错误消息以在安装失败时显示</span><span class="sxs-lookup"><span data-stu-id="6586d-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="6586d-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6586d-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="6586d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6586d-128">Int32</span></span>|<span data-ttu-id="6586d-129">设置安装进度超时（分钟）</span><span class="sxs-lookup"><span data-stu-id="6586d-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="6586d-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="6586d-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="6586d-131">布尔</span><span class="sxs-lookup"><span data-stu-id="6586d-131">Boolean</span></span>|<span data-ttu-id="6586d-132">允许用户在安装失败时继续使用设备</span><span class="sxs-lookup"><span data-stu-id="6586d-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="6586d-133">关系</span><span class="sxs-lookup"><span data-stu-id="6586d-133">Relationships</span></span>
<span data-ttu-id="6586d-134">无</span><span class="sxs-lookup"><span data-stu-id="6586d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6586d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6586d-135">JSON Representation</span></span>
<span data-ttu-id="6586d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6586d-136">Here is a JSON representation of the resource.</span></span>
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





