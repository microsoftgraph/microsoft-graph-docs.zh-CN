---
title: androidDeviceOwnerKioskCustomizationStatusBar 枚举类型
description: 表示展台自定义系统导航的可能值的枚举。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98eec7bcbce3093a05a8745629ca2793b72542d0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337012"
---
# <a name="androiddeviceownerkioskcustomizationstatusbar-enum-type"></a><span data-ttu-id="cb30e-103">androidDeviceOwnerKioskCustomizationStatusBar 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cb30e-103">androidDeviceOwnerKioskCustomizationStatusBar enum type</span></span>

<span data-ttu-id="cb30e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb30e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb30e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb30e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb30e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb30e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb30e-107">表示展台自定义系统导航的可能值的枚举。</span><span class="sxs-lookup"><span data-stu-id="cb30e-107">An enum representing possible values for kiosk customization system navigation.</span></span>

## <a name="members"></a><span data-ttu-id="cb30e-108">成员</span><span class="sxs-lookup"><span data-stu-id="cb30e-108">Members</span></span>
|<span data-ttu-id="cb30e-109">成员</span><span class="sxs-lookup"><span data-stu-id="cb30e-109">Member</span></span>|<span data-ttu-id="cb30e-110">值</span><span class="sxs-lookup"><span data-stu-id="cb30e-110">Value</span></span>|<span data-ttu-id="cb30e-111">Description</span><span class="sxs-lookup"><span data-stu-id="cb30e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb30e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cb30e-112">notConfigured</span></span>|<span data-ttu-id="cb30e-113">0</span><span class="sxs-lookup"><span data-stu-id="cb30e-113">0</span></span>|<span data-ttu-id="cb30e-114">未配置;此值默认为 STATUS_BAR_UNSPECIFIED。</span><span class="sxs-lookup"><span data-stu-id="cb30e-114">Not configured; this value defaults to STATUS_BAR_UNSPECIFIED.</span></span>|
|<span data-ttu-id="cb30e-115">notificationsAndSystemInfoEnabled</span><span class="sxs-lookup"><span data-stu-id="cb30e-115">notificationsAndSystemInfoEnabled</span></span>|<span data-ttu-id="cb30e-116">1</span><span class="sxs-lookup"><span data-stu-id="cb30e-116">1</span></span>|<span data-ttu-id="cb30e-117">"系统信息" 和 "通知" 显示在展台模式下的状态栏中。</span><span class="sxs-lookup"><span data-stu-id="cb30e-117">System info and notifications are shown on the status bar in kiosk mode.</span></span>|
|<span data-ttu-id="cb30e-118">systemInfoOnly</span><span class="sxs-lookup"><span data-stu-id="cb30e-118">systemInfoOnly</span></span>|<span data-ttu-id="cb30e-119">双面</span><span class="sxs-lookup"><span data-stu-id="cb30e-119">2</span></span>|<span data-ttu-id="cb30e-120">在展台模式下，仅在状态栏上显示 "系统信息"。</span><span class="sxs-lookup"><span data-stu-id="cb30e-120">Only system info is shown on the status bar in kiosk mode.</span></span>|




