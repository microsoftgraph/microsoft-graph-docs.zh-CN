---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2233c1dea3dfc8992becf1a12c8e99f1938020a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522074"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="898d6-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="898d6-103">managedDevice resource type</span></span>

> <span data-ttu-id="898d6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="898d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="898d6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="898d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="898d6-106">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="898d6-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="898d6-107">方法</span><span class="sxs-lookup"><span data-stu-id="898d6-107">Methods</span></span>
|<span data-ttu-id="898d6-108">方法</span><span class="sxs-lookup"><span data-stu-id="898d6-108">Method</span></span>|<span data-ttu-id="898d6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="898d6-109">Return Type</span></span>|<span data-ttu-id="898d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="898d6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="898d6-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="898d6-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="898d6-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="898d6-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="898d6-113">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="898d6-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="898d6-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="898d6-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="898d6-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="898d6-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="898d6-116">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="898d6-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="898d6-117">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="898d6-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="898d6-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="898d6-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="898d6-119">Not yet documented</span></span>|
|[<span data-ttu-id="898d6-120">enableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="898d6-121">无</span><span class="sxs-lookup"><span data-stu-id="898d6-121">None</span></span>|<span data-ttu-id="898d6-122">启用丢失模式</span><span class="sxs-lookup"><span data-stu-id="898d6-122">Enable lost mode</span></span>|
|[<span data-ttu-id="898d6-123">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="898d6-124">无</span><span class="sxs-lookup"><span data-stu-id="898d6-124">None</span></span>|<span data-ttu-id="898d6-125">远程锁定</span><span class="sxs-lookup"><span data-stu-id="898d6-125">Remote lock</span></span>|
|[<span data-ttu-id="898d6-126">setDeviceName 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="898d6-127">无</span><span class="sxs-lookup"><span data-stu-id="898d6-127">None</span></span>|<span data-ttu-id="898d6-128">设置设备的设备名称。</span><span class="sxs-lookup"><span data-stu-id="898d6-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="898d6-129">retire 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-129">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="898d6-130">无</span><span class="sxs-lookup"><span data-stu-id="898d6-130">None</span></span>|<span data-ttu-id="898d6-131">停用设备</span><span class="sxs-lookup"><span data-stu-id="898d6-131">Retire a device</span></span>|
|[<span data-ttu-id="898d6-132">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-132">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="898d6-133">无</span><span class="sxs-lookup"><span data-stu-id="898d6-133">None</span></span>|<span data-ttu-id="898d6-134">擦除设备</span><span class="sxs-lookup"><span data-stu-id="898d6-134">Wipe a device</span></span>|
|[<span data-ttu-id="898d6-135">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-135">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="898d6-136">无</span><span class="sxs-lookup"><span data-stu-id="898d6-136">None</span></span>|<span data-ttu-id="898d6-137">重置密码</span><span class="sxs-lookup"><span data-stu-id="898d6-137">Reset passcode</span></span>|
|[<span data-ttu-id="898d6-138">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-138">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="898d6-139">无</span><span class="sxs-lookup"><span data-stu-id="898d6-139">None</span></span>|<span data-ttu-id="898d6-140">远程锁定</span><span class="sxs-lookup"><span data-stu-id="898d6-140">Remote lock</span></span>|
|[<span data-ttu-id="898d6-141">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-141">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="898d6-142">无</span><span class="sxs-lookup"><span data-stu-id="898d6-142">None</span></span>|<span data-ttu-id="898d6-143">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="898d6-143">Request remote assistance</span></span>|
|[<span data-ttu-id="898d6-144">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-144">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="898d6-145">无</span><span class="sxs-lookup"><span data-stu-id="898d6-145">None</span></span>|<span data-ttu-id="898d6-146">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="898d6-146">Disable lost mode</span></span>|
|[<span data-ttu-id="898d6-147">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-147">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="898d6-148">无</span><span class="sxs-lookup"><span data-stu-id="898d6-148">None</span></span>|<span data-ttu-id="898d6-149">查找设备</span><span class="sxs-lookup"><span data-stu-id="898d6-149">Locate a device</span></span>|
|[<span data-ttu-id="898d6-150">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-150">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="898d6-151">无</span><span class="sxs-lookup"><span data-stu-id="898d6-151">None</span></span>|<span data-ttu-id="898d6-152">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="898d6-152">Bypass activation lock</span></span>|
|[<span data-ttu-id="898d6-153">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-153">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="898d6-154">无</span><span class="sxs-lookup"><span data-stu-id="898d6-154">None</span></span>|<span data-ttu-id="898d6-155">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="898d6-155">Reboot device</span></span>|
|[<span data-ttu-id="898d6-156">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-156">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="898d6-157">无</span><span class="sxs-lookup"><span data-stu-id="898d6-157">None</span></span>|<span data-ttu-id="898d6-158">关闭设备</span><span class="sxs-lookup"><span data-stu-id="898d6-158">Shut down device</span></span>|
|[<span data-ttu-id="898d6-159">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-159">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="898d6-160">无</span><span class="sxs-lookup"><span data-stu-id="898d6-160">None</span></span>|<span data-ttu-id="898d6-161">恢复密码</span><span class="sxs-lookup"><span data-stu-id="898d6-161">Recover passcode</span></span>|
|[<span data-ttu-id="898d6-162">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-162">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="898d6-163">无</span><span class="sxs-lookup"><span data-stu-id="898d6-163">None</span></span>|<span data-ttu-id="898d6-164">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="898d6-164">Clean Windows device</span></span>|
|[<span data-ttu-id="898d6-165">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-165">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="898d6-166">无</span><span class="sxs-lookup"><span data-stu-id="898d6-166">None</span></span>|<span data-ttu-id="898d6-167">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="898d6-167">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="898d6-168">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-168">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="898d6-169">无</span><span class="sxs-lookup"><span data-stu-id="898d6-169">None</span></span>|<span data-ttu-id="898d6-170">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="898d6-170">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="898d6-171">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-171">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="898d6-172">无</span><span class="sxs-lookup"><span data-stu-id="898d6-172">None</span></span>|<span data-ttu-id="898d6-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="898d6-173">Not yet documented</span></span>|
|[<span data-ttu-id="898d6-174">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-174">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="898d6-175">无</span><span class="sxs-lookup"><span data-stu-id="898d6-175">None</span></span>|<span data-ttu-id="898d6-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="898d6-176">Not yet documented</span></span>|
|[<span data-ttu-id="898d6-177">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-177">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="898d6-178">无</span><span class="sxs-lookup"><span data-stu-id="898d6-178">None</span></span>|<span data-ttu-id="898d6-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="898d6-179">Not yet documented</span></span>|
|[<span data-ttu-id="898d6-180">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-180">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="898d6-181">无</span><span class="sxs-lookup"><span data-stu-id="898d6-181">None</span></span>|<span data-ttu-id="898d6-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="898d6-182">Not yet documented</span></span>|
|[<span data-ttu-id="898d6-183">revokeAppleVppLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="898d6-183">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="898d6-184">无</span><span class="sxs-lookup"><span data-stu-id="898d6-184">None</span></span>|<span data-ttu-id="898d6-185">吊销设备的所有 Apple Vpp 许可证</span><span class="sxs-lookup"><span data-stu-id="898d6-185">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="898d6-186">属性</span><span class="sxs-lookup"><span data-stu-id="898d6-186">Properties</span></span>
|<span data-ttu-id="898d6-187">属性</span><span class="sxs-lookup"><span data-stu-id="898d6-187">Property</span></span>|<span data-ttu-id="898d6-188">类型</span><span class="sxs-lookup"><span data-stu-id="898d6-188">Type</span></span>|<span data-ttu-id="898d6-189">说明</span><span class="sxs-lookup"><span data-stu-id="898d6-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="898d6-190">id</span><span class="sxs-lookup"><span data-stu-id="898d6-190">id</span></span>|<span data-ttu-id="898d6-191">String</span><span class="sxs-lookup"><span data-stu-id="898d6-191">String</span></span>|<span data-ttu-id="898d6-192">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="898d6-192">Unique Identifier for the device</span></span>|
|<span data-ttu-id="898d6-193">userId</span><span class="sxs-lookup"><span data-stu-id="898d6-193">userId</span></span>|<span data-ttu-id="898d6-194">String</span><span class="sxs-lookup"><span data-stu-id="898d6-194">String</span></span>|<span data-ttu-id="898d6-195">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="898d6-195">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="898d6-196">deviceName</span><span class="sxs-lookup"><span data-stu-id="898d6-196">deviceName</span></span>|<span data-ttu-id="898d6-197">String</span><span class="sxs-lookup"><span data-stu-id="898d6-197">String</span></span>|<span data-ttu-id="898d6-198">设备的名称</span><span class="sxs-lookup"><span data-stu-id="898d6-198">Name of the device</span></span>|
|<span data-ttu-id="898d6-199">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="898d6-199">hardwareInformation</span></span>|[<span data-ttu-id="898d6-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="898d6-200">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="898d6-201">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="898d6-201">The hardward details for the device.</span></span>  <span data-ttu-id="898d6-202">包括存储空间、制造商、序列号等信息。</span><span class="sxs-lookup"><span data-stu-id="898d6-202">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="898d6-203">所有者</span><span class="sxs-lookup"><span data-stu-id="898d6-203">ownerType</span></span>|[<span data-ttu-id="898d6-204">所有者</span><span class="sxs-lookup"><span data-stu-id="898d6-204">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="898d6-205">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="898d6-205">Ownership of the device.</span></span> <span data-ttu-id="898d6-206">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="898d6-206">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="898d6-207">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="898d6-207">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="898d6-208">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="898d6-208">managedDeviceOwnerType</span></span>|[<span data-ttu-id="898d6-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="898d6-209">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="898d6-210">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="898d6-210">Ownership of the device.</span></span> <span data-ttu-id="898d6-211">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="898d6-211">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="898d6-212">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="898d6-212">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="898d6-213">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="898d6-213">deviceActionResults</span></span>|<span data-ttu-id="898d6-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898d6-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="898d6-215">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="898d6-215">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="898d6-216">managementState</span><span class="sxs-lookup"><span data-stu-id="898d6-216">managementState</span></span>|[<span data-ttu-id="898d6-217">managementState</span><span class="sxs-lookup"><span data-stu-id="898d6-217">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="898d6-218">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-218">Management state of the device.</span></span> <span data-ttu-id="898d6-219">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="898d6-219">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="898d6-220">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-220">enrolledDateTime</span></span>|<span data-ttu-id="898d6-221">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-221">DateTimeOffset</span></span>|<span data-ttu-id="898d6-222">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="898d6-222">Enrollment time of the device.</span></span>|
|<span data-ttu-id="898d6-223">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-223">lastSyncDateTime</span></span>|<span data-ttu-id="898d6-224">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-224">DateTimeOffset</span></span>|<span data-ttu-id="898d6-225">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="898d6-225">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="898d6-226">chassisType</span><span class="sxs-lookup"><span data-stu-id="898d6-226">chassisType</span></span>|[<span data-ttu-id="898d6-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="898d6-227">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="898d6-228">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="898d6-228">Chassis type of the device.</span></span> <span data-ttu-id="898d6-229">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="898d6-229">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="898d6-230">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="898d6-230">operatingSystem</span></span>|<span data-ttu-id="898d6-231">String</span><span class="sxs-lookup"><span data-stu-id="898d6-231">String</span></span>|<span data-ttu-id="898d6-232">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="898d6-232">Operating system of the device.</span></span> <span data-ttu-id="898d6-233">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="898d6-233">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="898d6-234">deviceType</span><span class="sxs-lookup"><span data-stu-id="898d6-234">deviceType</span></span>|[<span data-ttu-id="898d6-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="898d6-235">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="898d6-236">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="898d6-236">Platform of the device.</span></span> <span data-ttu-id="898d6-237">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="898d6-237">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="898d6-238">complianceState</span><span class="sxs-lookup"><span data-stu-id="898d6-238">complianceState</span></span>|[<span data-ttu-id="898d6-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="898d6-239">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="898d6-240">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-240">Compliance state of the device.</span></span> <span data-ttu-id="898d6-241">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="898d6-241">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="898d6-242">jailBroken</span><span class="sxs-lookup"><span data-stu-id="898d6-242">jailBroken</span></span>|<span data-ttu-id="898d6-243">String</span><span class="sxs-lookup"><span data-stu-id="898d6-243">String</span></span>|<span data-ttu-id="898d6-244">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="898d6-244">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="898d6-245">managementAgent</span><span class="sxs-lookup"><span data-stu-id="898d6-245">managementAgent</span></span>|[<span data-ttu-id="898d6-246">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="898d6-246">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="898d6-247">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="898d6-247">Management channel of the device.</span></span> <span data-ttu-id="898d6-248">Intune、EAS 等。可能的值为`eas`: `mdm`、 `easMdm`、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`、、、、、、、、 `microsoft365ManagedMdm` `jamf` `googleCloudDevicePolicyController`</span><span class="sxs-lookup"><span data-stu-id="898d6-248">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="898d6-249">osVersion</span><span class="sxs-lookup"><span data-stu-id="898d6-249">osVersion</span></span>|<span data-ttu-id="898d6-250">String</span><span class="sxs-lookup"><span data-stu-id="898d6-250">String</span></span>|<span data-ttu-id="898d6-251">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="898d6-251">Operating system version of the device.</span></span>|
|<span data-ttu-id="898d6-252">easActivated</span><span class="sxs-lookup"><span data-stu-id="898d6-252">easActivated</span></span>|<span data-ttu-id="898d6-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-253">Boolean</span></span>|<span data-ttu-id="898d6-254">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="898d6-254">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="898d6-255">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="898d6-255">easDeviceId</span></span>|<span data-ttu-id="898d6-256">String</span><span class="sxs-lookup"><span data-stu-id="898d6-256">String</span></span>|<span data-ttu-id="898d6-257">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="898d6-257">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="898d6-258">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-258">easActivationDateTime</span></span>|<span data-ttu-id="898d6-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-259">DateTimeOffset</span></span>|<span data-ttu-id="898d6-260">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="898d6-260">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="898d6-261">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="898d6-261">aadRegistered</span></span>|<span data-ttu-id="898d6-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-262">Boolean</span></span>|<span data-ttu-id="898d6-263">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="898d6-263">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="898d6-264">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="898d6-264">azureADRegistered</span></span>|<span data-ttu-id="898d6-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-265">Boolean</span></span>|<span data-ttu-id="898d6-266">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="898d6-266">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="898d6-267">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="898d6-267">deviceEnrollmentType</span></span>|[<span data-ttu-id="898d6-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="898d6-268">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="898d6-269">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="898d6-269">Enrollment type of the device.</span></span> <span data-ttu-id="898d6-270">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="898d6-270">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="898d6-271">lostModeState</span><span class="sxs-lookup"><span data-stu-id="898d6-271">lostModeState</span></span>|[<span data-ttu-id="898d6-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="898d6-272">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="898d6-273">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="898d6-273">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="898d6-274">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="898d6-274">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="898d6-275">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="898d6-275">activationLockBypassCode</span></span>|<span data-ttu-id="898d6-276">String</span><span class="sxs-lookup"><span data-stu-id="898d6-276">String</span></span>|<span data-ttu-id="898d6-277">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="898d6-277">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="898d6-278">emailAddress</span><span class="sxs-lookup"><span data-stu-id="898d6-278">emailAddress</span></span>|<span data-ttu-id="898d6-279">String</span><span class="sxs-lookup"><span data-stu-id="898d6-279">String</span></span>|<span data-ttu-id="898d6-280">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="898d6-280">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="898d6-281">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="898d6-281">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="898d6-282">String</span><span class="sxs-lookup"><span data-stu-id="898d6-282">String</span></span>|<span data-ttu-id="898d6-283">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="898d6-283">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="898d6-284">只读。</span><span class="sxs-lookup"><span data-stu-id="898d6-284">Read only.</span></span>|
|<span data-ttu-id="898d6-285">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="898d6-285">azureADDeviceId</span></span>|<span data-ttu-id="898d6-286">String</span><span class="sxs-lookup"><span data-stu-id="898d6-286">String</span></span>|<span data-ttu-id="898d6-287">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="898d6-287">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="898d6-288">只读。</span><span class="sxs-lookup"><span data-stu-id="898d6-288">Read only.</span></span>|
|<span data-ttu-id="898d6-289">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="898d6-289">deviceRegistrationState</span></span>|[<span data-ttu-id="898d6-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="898d6-290">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="898d6-291">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-291">Device registration state.</span></span> <span data-ttu-id="898d6-292">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="898d6-292">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="898d6-293">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="898d6-293">deviceCategoryDisplayName</span></span>|<span data-ttu-id="898d6-294">String</span><span class="sxs-lookup"><span data-stu-id="898d6-294">String</span></span>|<span data-ttu-id="898d6-295">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="898d6-295">Device category display name</span></span>|
|<span data-ttu-id="898d6-296">isSupervised</span><span class="sxs-lookup"><span data-stu-id="898d6-296">isSupervised</span></span>|<span data-ttu-id="898d6-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-297">Boolean</span></span>|<span data-ttu-id="898d6-298">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="898d6-298">Device supervised status</span></span>|
|<span data-ttu-id="898d6-299">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-299">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="898d6-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-300">DateTimeOffset</span></span>|<span data-ttu-id="898d6-301">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="898d6-301">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="898d6-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="898d6-302">exchangeAccessState</span></span>|[<span data-ttu-id="898d6-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="898d6-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="898d6-304">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="898d6-305">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="898d6-305">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="898d6-306">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="898d6-306">exchangeAccessStateReason</span></span>|[<span data-ttu-id="898d6-307">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="898d6-307">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="898d6-308">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="898d6-308">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="898d6-309">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="898d6-309">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="898d6-310">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="898d6-310">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="898d6-311">String</span><span class="sxs-lookup"><span data-stu-id="898d6-311">String</span></span>|<span data-ttu-id="898d6-312">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="898d6-312">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="898d6-313">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="898d6-313">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="898d6-314">String</span><span class="sxs-lookup"><span data-stu-id="898d6-314">String</span></span>|<span data-ttu-id="898d6-315">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="898d6-315">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="898d6-316">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="898d6-316">isEncrypted</span></span>|<span data-ttu-id="898d6-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-317">Boolean</span></span>|<span data-ttu-id="898d6-318">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="898d6-318">Device encryption status</span></span>|
|<span data-ttu-id="898d6-319">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="898d6-319">userPrincipalName</span></span>|<span data-ttu-id="898d6-320">String</span><span class="sxs-lookup"><span data-stu-id="898d6-320">String</span></span>|<span data-ttu-id="898d6-321">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="898d6-321">Device user principal name</span></span>|
|<span data-ttu-id="898d6-322">model</span><span class="sxs-lookup"><span data-stu-id="898d6-322">model</span></span>|<span data-ttu-id="898d6-323">String</span><span class="sxs-lookup"><span data-stu-id="898d6-323">String</span></span>|<span data-ttu-id="898d6-324">设备的型号</span><span class="sxs-lookup"><span data-stu-id="898d6-324">Model of the device</span></span>|
|<span data-ttu-id="898d6-325">manufacturer</span><span class="sxs-lookup"><span data-stu-id="898d6-325">manufacturer</span></span>|<span data-ttu-id="898d6-326">String</span><span class="sxs-lookup"><span data-stu-id="898d6-326">String</span></span>|<span data-ttu-id="898d6-327">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="898d6-327">Manufacturer of the device</span></span>|
|<span data-ttu-id="898d6-328">imei</span><span class="sxs-lookup"><span data-stu-id="898d6-328">imei</span></span>|<span data-ttu-id="898d6-329">String</span><span class="sxs-lookup"><span data-stu-id="898d6-329">String</span></span>|<span data-ttu-id="898d6-330">IMEI</span><span class="sxs-lookup"><span data-stu-id="898d6-330">IMEI</span></span>|
|<span data-ttu-id="898d6-331">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-331">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="898d6-332">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-332">DateTimeOffset</span></span>|<span data-ttu-id="898d6-333">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="898d6-333">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="898d6-334">serialNumber</span><span class="sxs-lookup"><span data-stu-id="898d6-334">serialNumber</span></span>|<span data-ttu-id="898d6-335">字符串</span><span class="sxs-lookup"><span data-stu-id="898d6-335">String</span></span>|<span data-ttu-id="898d6-336">序列号</span><span class="sxs-lookup"><span data-stu-id="898d6-336">SerialNumber</span></span>|
|<span data-ttu-id="898d6-337">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="898d6-337">phoneNumber</span></span>|<span data-ttu-id="898d6-338">String</span><span class="sxs-lookup"><span data-stu-id="898d6-338">String</span></span>|<span data-ttu-id="898d6-339">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="898d6-339">Phone number of the device</span></span>|
|<span data-ttu-id="898d6-340">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="898d6-340">androidSecurityPatchLevel</span></span>|<span data-ttu-id="898d6-341">String</span><span class="sxs-lookup"><span data-stu-id="898d6-341">String</span></span>|<span data-ttu-id="898d6-342">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="898d6-342">Android security patch level</span></span>|
|<span data-ttu-id="898d6-343">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="898d6-343">userDisplayName</span></span>|<span data-ttu-id="898d6-344">String</span><span class="sxs-lookup"><span data-stu-id="898d6-344">String</span></span>|<span data-ttu-id="898d6-345">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="898d6-345">User display name</span></span>|
|<span data-ttu-id="898d6-346">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="898d6-346">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="898d6-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="898d6-347">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="898d6-348">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="898d6-348">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="898d6-349">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="898d6-349">wiFiMacAddress</span></span>|<span data-ttu-id="898d6-350">String</span><span class="sxs-lookup"><span data-stu-id="898d6-350">String</span></span>|<span data-ttu-id="898d6-351">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="898d6-351">Wi-Fi MAC</span></span>|
|<span data-ttu-id="898d6-352">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="898d6-352">deviceHealthAttestationState</span></span>|[<span data-ttu-id="898d6-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="898d6-353">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="898d6-354">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-354">The device health attestation state.</span></span>|
|<span data-ttu-id="898d6-355">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="898d6-355">subscriberCarrier</span></span>|<span data-ttu-id="898d6-356">String</span><span class="sxs-lookup"><span data-stu-id="898d6-356">String</span></span>|<span data-ttu-id="898d6-357">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="898d6-357">Subscriber Carrier</span></span>|
|<span data-ttu-id="898d6-358">meid</span><span class="sxs-lookup"><span data-stu-id="898d6-358">meid</span></span>|<span data-ttu-id="898d6-359">String</span><span class="sxs-lookup"><span data-stu-id="898d6-359">String</span></span>|<span data-ttu-id="898d6-360">MEID</span><span class="sxs-lookup"><span data-stu-id="898d6-360">MEID</span></span>|
|<span data-ttu-id="898d6-361">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="898d6-361">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="898d6-362">Int64</span><span class="sxs-lookup"><span data-stu-id="898d6-362">Int64</span></span>|<span data-ttu-id="898d6-363">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="898d6-363">Total Storage in Bytes</span></span>|
|<span data-ttu-id="898d6-364">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="898d6-364">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="898d6-365">Int64</span><span class="sxs-lookup"><span data-stu-id="898d6-365">Int64</span></span>|<span data-ttu-id="898d6-366">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="898d6-366">Free Storage in Bytes</span></span>|
|<span data-ttu-id="898d6-367">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="898d6-367">managedDeviceName</span></span>|<span data-ttu-id="898d6-368">String</span><span class="sxs-lookup"><span data-stu-id="898d6-368">String</span></span>|<span data-ttu-id="898d6-369">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="898d6-369">Automatically generated name to identify a device.</span></span> <span data-ttu-id="898d6-370">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="898d6-370">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="898d6-371">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="898d6-371">partnerReportedThreatState</span></span>|[<span data-ttu-id="898d6-372">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="898d6-372">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="898d6-373">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-373">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="898d6-374">只读。</span><span class="sxs-lookup"><span data-stu-id="898d6-374">Read Only.</span></span> <span data-ttu-id="898d6-375">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="898d6-375">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="898d6-376">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="898d6-376">usersLoggedOn</span></span>|<span data-ttu-id="898d6-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="898d6-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="898d6-378">指示设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="898d6-378">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="898d6-379">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="898d6-379">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="898d6-380">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-380">DateTimeOffset</span></span>|<span data-ttu-id="898d6-381">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="898d6-381">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="898d6-382">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="898d6-382">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="898d6-383">只读。</span><span class="sxs-lookup"><span data-stu-id="898d6-383">Read Only.</span></span>|
|<span data-ttu-id="898d6-384">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="898d6-384">autopilotEnrolled</span></span>|<span data-ttu-id="898d6-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-385">Boolean</span></span>|<span data-ttu-id="898d6-386">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="898d6-386">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="898d6-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="898d6-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="898d6-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="898d6-388">Boolean</span></span>|<span data-ttu-id="898d6-389">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="898d6-389">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="898d6-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="898d6-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="898d6-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d6-391">DateTimeOffset</span></span>|<span data-ttu-id="898d6-392">报告设备管理证书到期日期</span><span class="sxs-lookup"><span data-stu-id="898d6-392">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="898d6-393">iccid</span><span class="sxs-lookup"><span data-stu-id="898d6-393">iccid</span></span>|<span data-ttu-id="898d6-394">String</span><span class="sxs-lookup"><span data-stu-id="898d6-394">String</span></span>|<span data-ttu-id="898d6-395">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="898d6-395">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="898d6-396">udid</span><span class="sxs-lookup"><span data-stu-id="898d6-396">udid</span></span>|<span data-ttu-id="898d6-397">String</span><span class="sxs-lookup"><span data-stu-id="898d6-397">String</span></span>|<span data-ttu-id="898d6-398">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="898d6-398">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="898d6-399">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="898d6-399">roleScopeTagIds</span></span>|<span data-ttu-id="898d6-400">String collection</span><span class="sxs-lookup"><span data-stu-id="898d6-400">String collection</span></span>|<span data-ttu-id="898d6-401">此设备实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="898d6-401">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="898d6-402">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="898d6-402">windowsActiveMalwareCount</span></span>|<span data-ttu-id="898d6-403">Int32</span><span class="sxs-lookup"><span data-stu-id="898d6-403">Int32</span></span>|<span data-ttu-id="898d6-404">此 windows 设备的活动恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="898d6-404">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="898d6-405">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="898d6-405">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="898d6-406">Int32</span><span class="sxs-lookup"><span data-stu-id="898d6-406">Int32</span></span>|<span data-ttu-id="898d6-407">此 windows 设备的修正的恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="898d6-407">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="898d6-408">notes</span><span class="sxs-lookup"><span data-stu-id="898d6-408">notes</span></span>|<span data-ttu-id="898d6-409">String</span><span class="sxs-lookup"><span data-stu-id="898d6-409">String</span></span>|<span data-ttu-id="898d6-410">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="898d6-410">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="898d6-411">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="898d6-411">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="898d6-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="898d6-412">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="898d6-413">Configuration manager 客户端运行状况状态, 仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="898d6-413">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="898d6-414">关系</span><span class="sxs-lookup"><span data-stu-id="898d6-414">Relationships</span></span>
|<span data-ttu-id="898d6-415">关系</span><span class="sxs-lookup"><span data-stu-id="898d6-415">Relationship</span></span>|<span data-ttu-id="898d6-416">类型</span><span class="sxs-lookup"><span data-stu-id="898d6-416">Type</span></span>|<span data-ttu-id="898d6-417">说明</span><span class="sxs-lookup"><span data-stu-id="898d6-417">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="898d6-418">detectedApps</span><span class="sxs-lookup"><span data-stu-id="898d6-418">detectedApps</span></span>|<span data-ttu-id="898d6-419">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898d6-419">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="898d6-420">设备上当前安装的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="898d6-420">All applications currently installed on the device</span></span>|
|<span data-ttu-id="898d6-421">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="898d6-421">deviceCategory</span></span>|[<span data-ttu-id="898d6-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="898d6-422">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="898d6-423">设备类别</span><span class="sxs-lookup"><span data-stu-id="898d6-423">Device category</span></span>|
|<span data-ttu-id="898d6-424">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="898d6-424">windowsProtectionState</span></span>|[<span data-ttu-id="898d6-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="898d6-425">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="898d6-426">设备保护状态。</span><span class="sxs-lookup"><span data-stu-id="898d6-426">The device protection status.</span></span>|
|<span data-ttu-id="898d6-427">users</span><span class="sxs-lookup"><span data-stu-id="898d6-427">users</span></span>|<span data-ttu-id="898d6-428">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898d6-428">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="898d6-429">与托管设备关联的主要用户。</span><span class="sxs-lookup"><span data-stu-id="898d6-429">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="898d6-430">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="898d6-430">JSON Representation</span></span>
<span data-ttu-id="898d6-431">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="898d6-431">Here is a JSON representation of the resource.</span></span>
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
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
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
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





