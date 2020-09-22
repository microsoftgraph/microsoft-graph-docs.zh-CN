---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75a968f6f0539c3f1c136c2e1127fae39d9f58c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091143"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="cd6c4-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd6c4-103">managedDevice resource type</span></span>

<span data-ttu-id="cd6c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd6c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd6c4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd6c4-106">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="cd6c4-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd6c4-107">Methods</span></span>
|<span data-ttu-id="cd6c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="cd6c4-108">Method</span></span>|<span data-ttu-id="cd6c4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd6c4-109">Return Type</span></span>|<span data-ttu-id="cd6c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd6c4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd6c4-111">List managedDevices</span><span class="sxs-lookup"><span data-stu-id="cd6c4-111">List managedDevices</span></span>](../api/intune-devices-manageddevice-list.md)|<span data-ttu-id="cd6c4-112">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6c4-112">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="cd6c4-113">列出 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-113">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="cd6c4-114">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-114">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="cd6c4-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="cd6c4-116">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-116">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="cd6c4-117">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-117">Create managedDevice</span></span>](../api/intune-devices-manageddevice-create.md)|[<span data-ttu-id="cd6c4-118">managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-118">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="cd6c4-119">创建新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-119">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="cd6c4-120">Delete managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-120">Delete managedDevice</span></span>](../api/intune-devices-manageddevice-delete.md)|<span data-ttu-id="cd6c4-121">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-121">None</span></span>|<span data-ttu-id="cd6c4-122">删除 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-122">Deletes a [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>|
|[<span data-ttu-id="cd6c4-123">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-123">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="cd6c4-124">managedDevice</span><span class="sxs-lookup"><span data-stu-id="cd6c4-124">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="cd6c4-125">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-125">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="cd6c4-126">retire 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-126">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="cd6c4-127">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-127">None</span></span>|<span data-ttu-id="cd6c4-128">停用设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-128">Retire a device</span></span>|
|[<span data-ttu-id="cd6c4-129">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-129">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="cd6c4-130">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-130">None</span></span>|<span data-ttu-id="cd6c4-131">擦除设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-131">Wipe a device</span></span>|
|[<span data-ttu-id="cd6c4-132">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-132">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="cd6c4-133">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-133">None</span></span>|<span data-ttu-id="cd6c4-134">重置密码</span><span class="sxs-lookup"><span data-stu-id="cd6c4-134">Reset passcode</span></span>|
|[<span data-ttu-id="cd6c4-135">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-135">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="cd6c4-136">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-136">None</span></span>|<span data-ttu-id="cd6c4-137">远程锁定</span><span class="sxs-lookup"><span data-stu-id="cd6c4-137">Remote lock</span></span>|
|[<span data-ttu-id="cd6c4-138">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-138">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="cd6c4-139">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-139">None</span></span>|<span data-ttu-id="cd6c4-140">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="cd6c4-140">Request remote assistance</span></span>|
|[<span data-ttu-id="cd6c4-141">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-141">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="cd6c4-142">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-142">None</span></span>|<span data-ttu-id="cd6c4-143">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="cd6c4-143">Disable lost mode</span></span>|
|[<span data-ttu-id="cd6c4-144">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-144">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="cd6c4-145">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-145">None</span></span>|<span data-ttu-id="cd6c4-146">查找设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-146">Locate a device</span></span>|
|[<span data-ttu-id="cd6c4-147">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-147">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="cd6c4-148">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-148">None</span></span>|<span data-ttu-id="cd6c4-149">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="cd6c4-149">Bypass activation lock</span></span>|
|[<span data-ttu-id="cd6c4-150">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-150">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="cd6c4-151">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-151">None</span></span>|<span data-ttu-id="cd6c4-152">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-152">Reboot device</span></span>|
|[<span data-ttu-id="cd6c4-153">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-153">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="cd6c4-154">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-154">None</span></span>|<span data-ttu-id="cd6c4-155">关闭设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-155">Shut down device</span></span>|
|[<span data-ttu-id="cd6c4-156">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-156">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="cd6c4-157">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-157">None</span></span>|<span data-ttu-id="cd6c4-158">恢复密码</span><span class="sxs-lookup"><span data-stu-id="cd6c4-158">Recover passcode</span></span>|
|[<span data-ttu-id="cd6c4-159">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-159">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="cd6c4-160">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-160">None</span></span>|<span data-ttu-id="cd6c4-161">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="cd6c4-161">Clean Windows device</span></span>|
|[<span data-ttu-id="cd6c4-162">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-162">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="cd6c4-163">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-163">None</span></span>|<span data-ttu-id="cd6c4-164">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="cd6c4-164">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="cd6c4-165">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-165">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="cd6c4-166">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-166">None</span></span>|<span data-ttu-id="cd6c4-167">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="cd6c4-167">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="cd6c4-168">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-168">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="cd6c4-169">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-169">None</span></span>|<span data-ttu-id="cd6c4-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd6c4-170">Not yet documented</span></span>|
|[<span data-ttu-id="cd6c4-171">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-171">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="cd6c4-172">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-172">None</span></span>|<span data-ttu-id="cd6c4-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd6c4-173">Not yet documented</span></span>|
|[<span data-ttu-id="cd6c4-174">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-174">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="cd6c4-175">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-175">None</span></span>|<span data-ttu-id="cd6c4-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd6c4-176">Not yet documented</span></span>|
|[<span data-ttu-id="cd6c4-177">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="cd6c4-177">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="cd6c4-178">无</span><span class="sxs-lookup"><span data-stu-id="cd6c4-178">None</span></span>|<span data-ttu-id="cd6c4-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd6c4-179">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cd6c4-180">属性</span><span class="sxs-lookup"><span data-stu-id="cd6c4-180">Properties</span></span>
|<span data-ttu-id="cd6c4-181">属性</span><span class="sxs-lookup"><span data-stu-id="cd6c4-181">Property</span></span>|<span data-ttu-id="cd6c4-182">类型</span><span class="sxs-lookup"><span data-stu-id="cd6c4-182">Type</span></span>|<span data-ttu-id="cd6c4-183">说明</span><span class="sxs-lookup"><span data-stu-id="cd6c4-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd6c4-184">id</span><span class="sxs-lookup"><span data-stu-id="cd6c4-184">id</span></span>|<span data-ttu-id="cd6c4-185">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-185">String</span></span>|<span data-ttu-id="cd6c4-186">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cd6c4-186">Unique Identifier for the device</span></span>|
|<span data-ttu-id="cd6c4-187">userId</span><span class="sxs-lookup"><span data-stu-id="cd6c4-187">userId</span></span>|<span data-ttu-id="cd6c4-188">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-188">String</span></span>|<span data-ttu-id="cd6c4-189">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cd6c4-189">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="cd6c4-190">deviceName</span><span class="sxs-lookup"><span data-stu-id="cd6c4-190">deviceName</span></span>|<span data-ttu-id="cd6c4-191">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-191">String</span></span>|<span data-ttu-id="cd6c4-192">设备的名称</span><span class="sxs-lookup"><span data-stu-id="cd6c4-192">Name of the device</span></span>|
|<span data-ttu-id="cd6c4-193">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="cd6c4-193">managedDeviceOwnerType</span></span>|[<span data-ttu-id="cd6c4-194">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="cd6c4-194">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="cd6c4-195">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-195">Ownership of the device.</span></span> <span data-ttu-id="cd6c4-196">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-196">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="cd6c4-197">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-197">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="cd6c4-198">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="cd6c4-198">deviceActionResults</span></span>|<span data-ttu-id="cd6c4-199">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6c4-199">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="cd6c4-200">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-200">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="cd6c4-201">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6c4-201">enrolledDateTime</span></span>|<span data-ttu-id="cd6c4-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6c4-202">DateTimeOffset</span></span>|<span data-ttu-id="cd6c4-203">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-203">Enrollment time of the device.</span></span>|
|<span data-ttu-id="cd6c4-204">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6c4-204">lastSyncDateTime</span></span>|<span data-ttu-id="cd6c4-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6c4-205">DateTimeOffset</span></span>|<span data-ttu-id="cd6c4-206">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-206">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="cd6c4-207">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="cd6c4-207">operatingSystem</span></span>|<span data-ttu-id="cd6c4-208">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-208">String</span></span>|<span data-ttu-id="cd6c4-209">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-209">Operating system of the device.</span></span> <span data-ttu-id="cd6c4-210">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-210">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="cd6c4-211">complianceState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-211">complianceState</span></span>|[<span data-ttu-id="cd6c4-212">complianceState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-212">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="cd6c4-213">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-213">Compliance state of the device.</span></span> <span data-ttu-id="cd6c4-214">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-214">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="cd6c4-215">jailBroken</span><span class="sxs-lookup"><span data-stu-id="cd6c4-215">jailBroken</span></span>|<span data-ttu-id="cd6c4-216">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-216">String</span></span>|<span data-ttu-id="cd6c4-217">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-217">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="cd6c4-218">managementAgent</span><span class="sxs-lookup"><span data-stu-id="cd6c4-218">managementAgent</span></span>|[<span data-ttu-id="cd6c4-219">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="cd6c4-219">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="cd6c4-220">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-220">Management channel of the device.</span></span> <span data-ttu-id="cd6c4-221">Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-221">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="cd6c4-222">osVersion</span><span class="sxs-lookup"><span data-stu-id="cd6c4-222">osVersion</span></span>|<span data-ttu-id="cd6c4-223">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-223">String</span></span>|<span data-ttu-id="cd6c4-224">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-224">Operating system version of the device.</span></span>|
|<span data-ttu-id="cd6c4-225">easActivated</span><span class="sxs-lookup"><span data-stu-id="cd6c4-225">easActivated</span></span>|<span data-ttu-id="cd6c4-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd6c4-226">Boolean</span></span>|<span data-ttu-id="cd6c4-227">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-227">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="cd6c4-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="cd6c4-228">easDeviceId</span></span>|<span data-ttu-id="cd6c4-229">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-229">String</span></span>|<span data-ttu-id="cd6c4-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-230">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="cd6c4-231">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6c4-231">easActivationDateTime</span></span>|<span data-ttu-id="cd6c4-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6c4-232">DateTimeOffset</span></span>|<span data-ttu-id="cd6c4-233">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-233">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="cd6c4-234">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="cd6c4-234">azureADRegistered</span></span>|<span data-ttu-id="cd6c4-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd6c4-235">Boolean</span></span>|<span data-ttu-id="cd6c4-236">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-236">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="cd6c4-237">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="cd6c4-237">deviceEnrollmentType</span></span>|[<span data-ttu-id="cd6c4-238">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="cd6c4-238">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="cd6c4-239">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-239">Enrollment type of the device.</span></span> <span data-ttu-id="cd6c4-240">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-240">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="cd6c4-241">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="cd6c4-241">activationLockBypassCode</span></span>|<span data-ttu-id="cd6c4-242">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-242">String</span></span>|<span data-ttu-id="cd6c4-243">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-243">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="cd6c4-244">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cd6c4-244">emailAddress</span></span>|<span data-ttu-id="cd6c4-245">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-245">String</span></span>|<span data-ttu-id="cd6c4-246">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-246">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="cd6c4-247">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="cd6c4-247">azureADDeviceId</span></span>|<span data-ttu-id="cd6c4-248">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-248">String</span></span>|<span data-ttu-id="cd6c4-249">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-249">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="cd6c4-250">只读。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-250">Read only.</span></span>|
|<span data-ttu-id="cd6c4-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-251">deviceRegistrationState</span></span>|[<span data-ttu-id="cd6c4-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="cd6c4-253">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-253">Device registration state.</span></span> <span data-ttu-id="cd6c4-254">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="cd6c4-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="cd6c4-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="cd6c4-256">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-256">String</span></span>|<span data-ttu-id="cd6c4-257">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-257">Device category display name</span></span>|
|<span data-ttu-id="cd6c4-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="cd6c4-258">isSupervised</span></span>|<span data-ttu-id="cd6c4-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd6c4-259">Boolean</span></span>|<span data-ttu-id="cd6c4-260">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="cd6c4-260">Device supervised status</span></span>|
|<span data-ttu-id="cd6c4-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6c4-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="cd6c4-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6c4-262">DateTimeOffset</span></span>|<span data-ttu-id="cd6c4-263">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-263">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="cd6c4-264">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-264">exchangeAccessState</span></span>|[<span data-ttu-id="cd6c4-265">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-265">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="cd6c4-266">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-266">The Access State of the device in Exchange.</span></span> <span data-ttu-id="cd6c4-267">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-267">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="cd6c4-268">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="cd6c4-268">exchangeAccessStateReason</span></span>|[<span data-ttu-id="cd6c4-269">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="cd6c4-269">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="cd6c4-270">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-270">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="cd6c4-271">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-271">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="cd6c4-272">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="cd6c4-272">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="cd6c4-273">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-273">String</span></span>|<span data-ttu-id="cd6c4-274">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-274">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="cd6c4-275">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cd6c4-275">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="cd6c4-276">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-276">String</span></span>|<span data-ttu-id="cd6c4-277">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-277">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="cd6c4-278">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="cd6c4-278">isEncrypted</span></span>|<span data-ttu-id="cd6c4-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd6c4-279">Boolean</span></span>|<span data-ttu-id="cd6c4-280">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="cd6c4-280">Device encryption status</span></span>|
|<span data-ttu-id="cd6c4-281">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd6c4-281">userPrincipalName</span></span>|<span data-ttu-id="cd6c4-282">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-282">String</span></span>|<span data-ttu-id="cd6c4-283">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="cd6c4-283">Device user principal name</span></span>|
|<span data-ttu-id="cd6c4-284">model</span><span class="sxs-lookup"><span data-stu-id="cd6c4-284">model</span></span>|<span data-ttu-id="cd6c4-285">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-285">String</span></span>|<span data-ttu-id="cd6c4-286">设备的型号</span><span class="sxs-lookup"><span data-stu-id="cd6c4-286">Model of the device</span></span>|
|<span data-ttu-id="cd6c4-287">manufacturer</span><span class="sxs-lookup"><span data-stu-id="cd6c4-287">manufacturer</span></span>|<span data-ttu-id="cd6c4-288">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-288">String</span></span>|<span data-ttu-id="cd6c4-289">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="cd6c4-289">Manufacturer of the device</span></span>|
|<span data-ttu-id="cd6c4-290">imei</span><span class="sxs-lookup"><span data-stu-id="cd6c4-290">imei</span></span>|<span data-ttu-id="cd6c4-291">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-291">String</span></span>|<span data-ttu-id="cd6c4-292">IMEI</span><span class="sxs-lookup"><span data-stu-id="cd6c4-292">IMEI</span></span>|
|<span data-ttu-id="cd6c4-293">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd6c4-293">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="cd6c4-294">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd6c4-294">DateTimeOffset</span></span>|<span data-ttu-id="cd6c4-295">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="cd6c4-295">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="cd6c4-296">serialNumber</span><span class="sxs-lookup"><span data-stu-id="cd6c4-296">serialNumber</span></span>|<span data-ttu-id="cd6c4-297">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-297">String</span></span>|<span data-ttu-id="cd6c4-298">序列号</span><span class="sxs-lookup"><span data-stu-id="cd6c4-298">SerialNumber</span></span>|
|<span data-ttu-id="cd6c4-299">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="cd6c4-299">phoneNumber</span></span>|<span data-ttu-id="cd6c4-300">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-300">String</span></span>|<span data-ttu-id="cd6c4-301">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="cd6c4-301">Phone number of the device</span></span>|
|<span data-ttu-id="cd6c4-302">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="cd6c4-302">androidSecurityPatchLevel</span></span>|<span data-ttu-id="cd6c4-303">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-303">String</span></span>|<span data-ttu-id="cd6c4-304">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="cd6c4-304">Android security patch level</span></span>|
|<span data-ttu-id="cd6c4-305">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cd6c4-305">userDisplayName</span></span>|<span data-ttu-id="cd6c4-306">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-306">String</span></span>|<span data-ttu-id="cd6c4-307">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="cd6c4-307">User display name</span></span>|
|<span data-ttu-id="cd6c4-308">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="cd6c4-308">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="cd6c4-309">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="cd6c4-309">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="cd6c4-310">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="cd6c4-310">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="cd6c4-311">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="cd6c4-311">wiFiMacAddress</span></span>|<span data-ttu-id="cd6c4-312">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-312">String</span></span>|<span data-ttu-id="cd6c4-313">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="cd6c4-313">Wi-Fi MAC</span></span>|
|<span data-ttu-id="cd6c4-314">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-314">deviceHealthAttestationState</span></span>|[<span data-ttu-id="cd6c4-315">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-315">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="cd6c4-316">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-316">The device health attestation state.</span></span>|
|<span data-ttu-id="cd6c4-317">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="cd6c4-317">subscriberCarrier</span></span>|<span data-ttu-id="cd6c4-318">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-318">String</span></span>|<span data-ttu-id="cd6c4-319">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="cd6c4-319">Subscriber Carrier</span></span>|
|<span data-ttu-id="cd6c4-320">meid</span><span class="sxs-lookup"><span data-stu-id="cd6c4-320">meid</span></span>|<span data-ttu-id="cd6c4-321">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-321">String</span></span>|<span data-ttu-id="cd6c4-322">MEID</span><span class="sxs-lookup"><span data-stu-id="cd6c4-322">MEID</span></span>|
|<span data-ttu-id="cd6c4-323">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="cd6c4-323">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="cd6c4-324">Int64</span><span class="sxs-lookup"><span data-stu-id="cd6c4-324">Int64</span></span>|<span data-ttu-id="cd6c4-325">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="cd6c4-325">Total Storage in Bytes</span></span>|
|<span data-ttu-id="cd6c4-326">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="cd6c4-326">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="cd6c4-327">Int64</span><span class="sxs-lookup"><span data-stu-id="cd6c4-327">Int64</span></span>|<span data-ttu-id="cd6c4-328">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="cd6c4-328">Free Storage in Bytes</span></span>|
|<span data-ttu-id="cd6c4-329">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="cd6c4-329">managedDeviceName</span></span>|<span data-ttu-id="cd6c4-330">String</span><span class="sxs-lookup"><span data-stu-id="cd6c4-330">String</span></span>|<span data-ttu-id="cd6c4-331">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-331">Automatically generated name to identify a device.</span></span> <span data-ttu-id="cd6c4-332">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-332">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="cd6c4-333">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-333">partnerReportedThreatState</span></span>|[<span data-ttu-id="cd6c4-334">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="cd6c4-334">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="cd6c4-335">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-335">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="cd6c4-336">只读。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-336">Read Only.</span></span> <span data-ttu-id="cd6c4-337">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-337">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd6c4-338">关系</span><span class="sxs-lookup"><span data-stu-id="cd6c4-338">Relationships</span></span>
|<span data-ttu-id="cd6c4-339">关系</span><span class="sxs-lookup"><span data-stu-id="cd6c4-339">Relationship</span></span>|<span data-ttu-id="cd6c4-340">类型</span><span class="sxs-lookup"><span data-stu-id="cd6c4-340">Type</span></span>|<span data-ttu-id="cd6c4-341">说明</span><span class="sxs-lookup"><span data-stu-id="cd6c4-341">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd6c4-342">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cd6c4-342">deviceCategory</span></span>|[<span data-ttu-id="cd6c4-343">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cd6c4-343">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="cd6c4-344">设备类别</span><span class="sxs-lookup"><span data-stu-id="cd6c4-344">Device category</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd6c4-345">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd6c4-345">JSON Representation</span></span>
<span data-ttu-id="cd6c4-346">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd6c4-346">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```









