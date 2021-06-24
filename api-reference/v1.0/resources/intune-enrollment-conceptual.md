---
title: 使用 Intune 注册公司设备 - Microsoft Graph API
description: 列出为租户Graph注册设备的适用于 Intune (REST) 的 Microsoft Graph API。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daefbf23d8aa70cdd3f81fdcb4afb69dd2590ba7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108935"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="7b636-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="7b636-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="7b636-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b636-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b636-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b636-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b636-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b636-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b636-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b636-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b636-108">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="7b636-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="7b636-109">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="7b636-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="7b636-110">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="7b636-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="7b636-111">设备管理</span><span class="sxs-lookup"><span data-stu-id="7b636-111">Device management</span></span>](intune-enrollment-devicemanagement.md)
- [<span data-ttu-id="7b636-112">注册状态</span><span class="sxs-lookup"><span data-stu-id="7b636-112">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="7b636-113">已导入的 Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="7b636-113">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="7b636-114">已导入的 Windows Autopilot 设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="7b636-114">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="7b636-115">已导入的 Windows Autopilot 设备标识状态</span><span class="sxs-lookup"><span data-stu-id="7b636-115">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="7b636-116">已导入的 Windows Autopilot 设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="7b636-116">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="7b636-117">Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="7b636-117">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)