---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc519337284ac35d344876288826cf29a735da38
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407003"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="2ad99-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ad99-103">managedDevice resource type</span></span>

<span data-ttu-id="2ad99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ad99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ad99-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ad99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad99-106">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="2ad99-107">方法</span><span class="sxs-lookup"><span data-stu-id="2ad99-107">Methods</span></span>
|<span data-ttu-id="2ad99-108">方法</span><span class="sxs-lookup"><span data-stu-id="2ad99-108">Method</span></span>|<span data-ttu-id="2ad99-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ad99-109">Return Type</span></span>|<span data-ttu-id="2ad99-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ad99-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ad99-111">List managedDevices</span><span class="sxs-lookup"><span data-stu-id="2ad99-111">List managedDevices</span></span>](../api/intune-devices-manageddevice-list.md)|<span data-ttu-id="2ad99-112">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ad99-112">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="2ad99-113">列出 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ad99-113">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="2ad99-114">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-114">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="2ad99-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="2ad99-116">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ad99-116">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="2ad99-117">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-117">Create managedDevice</span></span>](../api/intune-devices-manageddevice-create.md)|[<span data-ttu-id="2ad99-118">managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-118">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="2ad99-119">创建新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ad99-119">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="2ad99-120">Delete managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-120">Delete managedDevice</span></span>](../api/intune-devices-manageddevice-delete.md)|<span data-ttu-id="2ad99-121">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-121">None</span></span>|<span data-ttu-id="2ad99-122">删除 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="2ad99-122">Deletes a [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>|
|[<span data-ttu-id="2ad99-123">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-123">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="2ad99-124">managedDevice</span><span class="sxs-lookup"><span data-stu-id="2ad99-124">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="2ad99-125">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2ad99-125">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="2ad99-126">retire 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-126">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="2ad99-127">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-127">None</span></span>|<span data-ttu-id="2ad99-128">停用设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-128">Retire a device</span></span>|
|[<span data-ttu-id="2ad99-129">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-129">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="2ad99-130">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-130">None</span></span>|<span data-ttu-id="2ad99-131">擦除设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-131">Wipe a device</span></span>|
|[<span data-ttu-id="2ad99-132">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-132">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="2ad99-133">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-133">None</span></span>|<span data-ttu-id="2ad99-134">重置密码</span><span class="sxs-lookup"><span data-stu-id="2ad99-134">Reset passcode</span></span>|
|[<span data-ttu-id="2ad99-135">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-135">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="2ad99-136">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-136">None</span></span>|<span data-ttu-id="2ad99-137">远程锁定</span><span class="sxs-lookup"><span data-stu-id="2ad99-137">Remote lock</span></span>|
|[<span data-ttu-id="2ad99-138">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-138">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="2ad99-139">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-139">None</span></span>|<span data-ttu-id="2ad99-140">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="2ad99-140">Request remote assistance</span></span>|
|[<span data-ttu-id="2ad99-141">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-141">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="2ad99-142">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-142">None</span></span>|<span data-ttu-id="2ad99-143">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="2ad99-143">Disable lost mode</span></span>|
|[<span data-ttu-id="2ad99-144">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-144">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="2ad99-145">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-145">None</span></span>|<span data-ttu-id="2ad99-146">查找设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-146">Locate a device</span></span>|
|[<span data-ttu-id="2ad99-147">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-147">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="2ad99-148">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-148">None</span></span>|<span data-ttu-id="2ad99-149">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="2ad99-149">Bypass activation lock</span></span>|
|[<span data-ttu-id="2ad99-150">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-150">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="2ad99-151">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-151">None</span></span>|<span data-ttu-id="2ad99-152">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-152">Reboot device</span></span>|
|[<span data-ttu-id="2ad99-153">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-153">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="2ad99-154">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-154">None</span></span>|<span data-ttu-id="2ad99-155">关闭设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-155">Shut down device</span></span>|
|[<span data-ttu-id="2ad99-156">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-156">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="2ad99-157">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-157">None</span></span>|<span data-ttu-id="2ad99-158">恢复密码</span><span class="sxs-lookup"><span data-stu-id="2ad99-158">Recover passcode</span></span>|
|[<span data-ttu-id="2ad99-159">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-159">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="2ad99-160">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-160">None</span></span>|<span data-ttu-id="2ad99-161">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="2ad99-161">Clean Windows device</span></span>|
|[<span data-ttu-id="2ad99-162">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-162">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="2ad99-163">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-163">None</span></span>|<span data-ttu-id="2ad99-164">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="2ad99-164">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="2ad99-165">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-165">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="2ad99-166">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-166">None</span></span>|<span data-ttu-id="2ad99-167">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="2ad99-167">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="2ad99-168">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-168">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="2ad99-169">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-169">None</span></span>|<span data-ttu-id="2ad99-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ad99-170">Not yet documented</span></span>|
|[<span data-ttu-id="2ad99-171">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-171">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="2ad99-172">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-172">None</span></span>|<span data-ttu-id="2ad99-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ad99-173">Not yet documented</span></span>|
|[<span data-ttu-id="2ad99-174">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-174">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="2ad99-175">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-175">None</span></span>|<span data-ttu-id="2ad99-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ad99-176">Not yet documented</span></span>|
|[<span data-ttu-id="2ad99-177">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="2ad99-177">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="2ad99-178">无</span><span class="sxs-lookup"><span data-stu-id="2ad99-178">None</span></span>|<span data-ttu-id="2ad99-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2ad99-179">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ad99-180">属性</span><span class="sxs-lookup"><span data-stu-id="2ad99-180">Properties</span></span>
|<span data-ttu-id="2ad99-181">属性</span><span class="sxs-lookup"><span data-stu-id="2ad99-181">Property</span></span>|<span data-ttu-id="2ad99-182">类型</span><span class="sxs-lookup"><span data-stu-id="2ad99-182">Type</span></span>|<span data-ttu-id="2ad99-183">说明</span><span class="sxs-lookup"><span data-stu-id="2ad99-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad99-184">id</span><span class="sxs-lookup"><span data-stu-id="2ad99-184">id</span></span>|<span data-ttu-id="2ad99-185">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad99-185">String</span></span>|<span data-ttu-id="2ad99-186">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="2ad99-186">Unique Identifier for the device</span></span>|
|<span data-ttu-id="2ad99-187">userId</span><span class="sxs-lookup"><span data-stu-id="2ad99-187">userId</span></span>|<span data-ttu-id="2ad99-188">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-188">String</span></span>|<span data-ttu-id="2ad99-189">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="2ad99-189">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="2ad99-190">deviceName</span><span class="sxs-lookup"><span data-stu-id="2ad99-190">deviceName</span></span>|<span data-ttu-id="2ad99-191">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-191">String</span></span>|<span data-ttu-id="2ad99-192">设备的名称</span><span class="sxs-lookup"><span data-stu-id="2ad99-192">Name of the device</span></span>|
|<span data-ttu-id="2ad99-193">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="2ad99-193">managedDeviceOwnerType</span></span>|[<span data-ttu-id="2ad99-194">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="2ad99-194">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="2ad99-195">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="2ad99-195">Ownership of the device.</span></span> <span data-ttu-id="2ad99-196">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="2ad99-196">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="2ad99-197">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-197">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="2ad99-198">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="2ad99-198">deviceActionResults</span></span>|<span data-ttu-id="2ad99-199">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ad99-199">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="2ad99-200">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2ad99-200">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="2ad99-201">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad99-201">enrolledDateTime</span></span>|<span data-ttu-id="2ad99-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad99-202">DateTimeOffset</span></span>|<span data-ttu-id="2ad99-203">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="2ad99-203">Enrollment time of the device.</span></span>|
|<span data-ttu-id="2ad99-204">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad99-204">lastSyncDateTime</span></span>|<span data-ttu-id="2ad99-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad99-205">DateTimeOffset</span></span>|<span data-ttu-id="2ad99-206">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ad99-206">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="2ad99-207">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ad99-207">operatingSystem</span></span>|<span data-ttu-id="2ad99-208">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-208">String</span></span>|<span data-ttu-id="2ad99-209">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="2ad99-209">Operating system of the device.</span></span> <span data-ttu-id="2ad99-210">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="2ad99-210">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="2ad99-211">complianceState</span><span class="sxs-lookup"><span data-stu-id="2ad99-211">complianceState</span></span>|[<span data-ttu-id="2ad99-212">complianceState</span><span class="sxs-lookup"><span data-stu-id="2ad99-212">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="2ad99-213">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2ad99-213">Compliance state of the device.</span></span> <span data-ttu-id="2ad99-214">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-214">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="2ad99-215">jailBroken</span><span class="sxs-lookup"><span data-stu-id="2ad99-215">jailBroken</span></span>|<span data-ttu-id="2ad99-216">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-216">String</span></span>|<span data-ttu-id="2ad99-217">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="2ad99-217">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="2ad99-218">managementAgent</span><span class="sxs-lookup"><span data-stu-id="2ad99-218">managementAgent</span></span>|[<span data-ttu-id="2ad99-219">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="2ad99-219">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="2ad99-220">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="2ad99-220">Management channel of the device.</span></span> <span data-ttu-id="2ad99-221">Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-221">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="2ad99-222">osVersion</span><span class="sxs-lookup"><span data-stu-id="2ad99-222">osVersion</span></span>|<span data-ttu-id="2ad99-223">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-223">String</span></span>|<span data-ttu-id="2ad99-224">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2ad99-224">Operating system version of the device.</span></span>|
|<span data-ttu-id="2ad99-225">easActivated</span><span class="sxs-lookup"><span data-stu-id="2ad99-225">easActivated</span></span>|<span data-ttu-id="2ad99-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad99-226">Boolean</span></span>|<span data-ttu-id="2ad99-227">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="2ad99-227">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="2ad99-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="2ad99-228">easDeviceId</span></span>|<span data-ttu-id="2ad99-229">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-229">String</span></span>|<span data-ttu-id="2ad99-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="2ad99-230">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="2ad99-231">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad99-231">easActivationDateTime</span></span>|<span data-ttu-id="2ad99-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad99-232">DateTimeOffset</span></span>|<span data-ttu-id="2ad99-233">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="2ad99-233">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="2ad99-234">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="2ad99-234">azureADRegistered</span></span>|<span data-ttu-id="2ad99-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad99-235">Boolean</span></span>|<span data-ttu-id="2ad99-236">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="2ad99-236">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="2ad99-237">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="2ad99-237">deviceEnrollmentType</span></span>|[<span data-ttu-id="2ad99-238">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="2ad99-238">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="2ad99-239">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="2ad99-239">Enrollment type of the device.</span></span> <span data-ttu-id="2ad99-240">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-240">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="2ad99-241">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="2ad99-241">activationLockBypassCode</span></span>|<span data-ttu-id="2ad99-242">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-242">String</span></span>|<span data-ttu-id="2ad99-243">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="2ad99-243">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="2ad99-244">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2ad99-244">emailAddress</span></span>|<span data-ttu-id="2ad99-245">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-245">String</span></span>|<span data-ttu-id="2ad99-246">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2ad99-246">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="2ad99-247">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="2ad99-247">azureADDeviceId</span></span>|<span data-ttu-id="2ad99-248">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-248">String</span></span>|<span data-ttu-id="2ad99-249">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2ad99-249">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="2ad99-250">只读。</span><span class="sxs-lookup"><span data-stu-id="2ad99-250">Read only.</span></span>|
|<span data-ttu-id="2ad99-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2ad99-251">deviceRegistrationState</span></span>|[<span data-ttu-id="2ad99-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2ad99-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="2ad99-253">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="2ad99-253">Device registration state.</span></span> <span data-ttu-id="2ad99-254">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="2ad99-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ad99-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="2ad99-256">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-256">String</span></span>|<span data-ttu-id="2ad99-257">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ad99-257">Device category display name</span></span>|
|<span data-ttu-id="2ad99-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="2ad99-258">isSupervised</span></span>|<span data-ttu-id="2ad99-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad99-259">Boolean</span></span>|<span data-ttu-id="2ad99-260">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="2ad99-260">Device supervised status</span></span>|
|<span data-ttu-id="2ad99-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad99-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="2ad99-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad99-262">DateTimeOffset</span></span>|<span data-ttu-id="2ad99-263">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="2ad99-263">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="2ad99-264">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="2ad99-264">exchangeAccessState</span></span>|[<span data-ttu-id="2ad99-265">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="2ad99-265">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="2ad99-266">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="2ad99-266">The Access State of the device in Exchange.</span></span> <span data-ttu-id="2ad99-267">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-267">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="2ad99-268">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="2ad99-268">exchangeAccessStateReason</span></span>|[<span data-ttu-id="2ad99-269">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="2ad99-269">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="2ad99-270">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="2ad99-270">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="2ad99-271">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-271">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="2ad99-272">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="2ad99-272">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="2ad99-273">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-273">String</span></span>|<span data-ttu-id="2ad99-274">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="2ad99-274">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="2ad99-275">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="2ad99-275">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="2ad99-276">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-276">String</span></span>|<span data-ttu-id="2ad99-277">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="2ad99-277">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="2ad99-278">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="2ad99-278">isEncrypted</span></span>|<span data-ttu-id="2ad99-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad99-279">Boolean</span></span>|<span data-ttu-id="2ad99-280">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="2ad99-280">Device encryption status</span></span>|
|<span data-ttu-id="2ad99-281">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ad99-281">userPrincipalName</span></span>|<span data-ttu-id="2ad99-282">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-282">String</span></span>|<span data-ttu-id="2ad99-283">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2ad99-283">Device user principal name</span></span>|
|<span data-ttu-id="2ad99-284">model</span><span class="sxs-lookup"><span data-stu-id="2ad99-284">model</span></span>|<span data-ttu-id="2ad99-285">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-285">String</span></span>|<span data-ttu-id="2ad99-286">设备的型号</span><span class="sxs-lookup"><span data-stu-id="2ad99-286">Model of the device</span></span>|
|<span data-ttu-id="2ad99-287">manufacturer</span><span class="sxs-lookup"><span data-stu-id="2ad99-287">manufacturer</span></span>|<span data-ttu-id="2ad99-288">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-288">String</span></span>|<span data-ttu-id="2ad99-289">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="2ad99-289">Manufacturer of the device</span></span>|
|<span data-ttu-id="2ad99-290">imei</span><span class="sxs-lookup"><span data-stu-id="2ad99-290">imei</span></span>|<span data-ttu-id="2ad99-291">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-291">String</span></span>|<span data-ttu-id="2ad99-292">IMEI</span><span class="sxs-lookup"><span data-stu-id="2ad99-292">IMEI</span></span>|
|<span data-ttu-id="2ad99-293">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad99-293">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2ad99-294">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad99-294">DateTimeOffset</span></span>|<span data-ttu-id="2ad99-295">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="2ad99-295">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2ad99-296">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2ad99-296">serialNumber</span></span>|<span data-ttu-id="2ad99-297">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad99-297">String</span></span>|<span data-ttu-id="2ad99-298">序列号</span><span class="sxs-lookup"><span data-stu-id="2ad99-298">SerialNumber</span></span>|
|<span data-ttu-id="2ad99-299">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="2ad99-299">phoneNumber</span></span>|<span data-ttu-id="2ad99-300">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-300">String</span></span>|<span data-ttu-id="2ad99-301">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="2ad99-301">Phone number of the device</span></span>|
|<span data-ttu-id="2ad99-302">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="2ad99-302">androidSecurityPatchLevel</span></span>|<span data-ttu-id="2ad99-303">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-303">String</span></span>|<span data-ttu-id="2ad99-304">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="2ad99-304">Android security patch level</span></span>|
|<span data-ttu-id="2ad99-305">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ad99-305">userDisplayName</span></span>|<span data-ttu-id="2ad99-306">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-306">String</span></span>|<span data-ttu-id="2ad99-307">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="2ad99-307">User display name</span></span>|
|<span data-ttu-id="2ad99-308">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2ad99-308">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="2ad99-309">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2ad99-309">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="2ad99-310">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="2ad99-310">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="2ad99-311">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="2ad99-311">wiFiMacAddress</span></span>|<span data-ttu-id="2ad99-312">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-312">String</span></span>|<span data-ttu-id="2ad99-313">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="2ad99-313">Wi-Fi MAC</span></span>|
|<span data-ttu-id="2ad99-314">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="2ad99-314">deviceHealthAttestationState</span></span>|[<span data-ttu-id="2ad99-315">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="2ad99-315">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="2ad99-316">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="2ad99-316">The device health attestation state.</span></span>|
|<span data-ttu-id="2ad99-317">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="2ad99-317">subscriberCarrier</span></span>|<span data-ttu-id="2ad99-318">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-318">String</span></span>|<span data-ttu-id="2ad99-319">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="2ad99-319">Subscriber Carrier</span></span>|
|<span data-ttu-id="2ad99-320">meid</span><span class="sxs-lookup"><span data-stu-id="2ad99-320">meid</span></span>|<span data-ttu-id="2ad99-321">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-321">String</span></span>|<span data-ttu-id="2ad99-322">MEID</span><span class="sxs-lookup"><span data-stu-id="2ad99-322">MEID</span></span>|
|<span data-ttu-id="2ad99-323">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="2ad99-323">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="2ad99-324">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad99-324">Int64</span></span>|<span data-ttu-id="2ad99-325">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="2ad99-325">Total Storage in Bytes</span></span>|
|<span data-ttu-id="2ad99-326">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="2ad99-326">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="2ad99-327">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad99-327">Int64</span></span>|<span data-ttu-id="2ad99-328">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="2ad99-328">Free Storage in Bytes</span></span>|
|<span data-ttu-id="2ad99-329">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="2ad99-329">managedDeviceName</span></span>|<span data-ttu-id="2ad99-330">String</span><span class="sxs-lookup"><span data-stu-id="2ad99-330">String</span></span>|<span data-ttu-id="2ad99-331">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="2ad99-331">Automatically generated name to identify a device.</span></span> <span data-ttu-id="2ad99-332">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="2ad99-332">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="2ad99-333">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="2ad99-333">partnerReportedThreatState</span></span>|[<span data-ttu-id="2ad99-334">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="2ad99-334">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="2ad99-335">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="2ad99-335">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="2ad99-336">只读。</span><span class="sxs-lookup"><span data-stu-id="2ad99-336">Read Only.</span></span> <span data-ttu-id="2ad99-337">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="2ad99-337">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ad99-338">关系</span><span class="sxs-lookup"><span data-stu-id="2ad99-338">Relationships</span></span>
|<span data-ttu-id="2ad99-339">关系</span><span class="sxs-lookup"><span data-stu-id="2ad99-339">Relationship</span></span>|<span data-ttu-id="2ad99-340">类型</span><span class="sxs-lookup"><span data-stu-id="2ad99-340">Type</span></span>|<span data-ttu-id="2ad99-341">说明</span><span class="sxs-lookup"><span data-stu-id="2ad99-341">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad99-342">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2ad99-342">deviceCategory</span></span>|[<span data-ttu-id="2ad99-343">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2ad99-343">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="2ad99-344">设备类别</span><span class="sxs-lookup"><span data-stu-id="2ad99-344">Device category</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ad99-345">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ad99-345">JSON Representation</span></span>
<span data-ttu-id="2ad99-346">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ad99-346">Here is a JSON representation of the resource.</span></span>
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







