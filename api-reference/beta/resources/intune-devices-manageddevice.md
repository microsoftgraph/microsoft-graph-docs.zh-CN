---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee7fd96654fe0b6c2a95332b87287d3ebff3ad2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995117"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="20929-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="20929-103">managedDevice resource type</span></span>

> <span data-ttu-id="20929-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20929-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20929-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20929-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20929-106">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="20929-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="20929-107">方法</span><span class="sxs-lookup"><span data-stu-id="20929-107">Methods</span></span>
|<span data-ttu-id="20929-108">方法</span><span class="sxs-lookup"><span data-stu-id="20929-108">Method</span></span>|<span data-ttu-id="20929-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="20929-109">Return Type</span></span>|<span data-ttu-id="20929-110">说明</span><span class="sxs-lookup"><span data-stu-id="20929-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20929-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="20929-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="20929-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="20929-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="20929-113">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="20929-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="20929-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="20929-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="20929-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="20929-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="20929-116">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20929-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="20929-117">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="20929-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="20929-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="20929-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="20929-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-119">Not yet documented</span></span>|
|[<span data-ttu-id="20929-120">enableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="20929-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="20929-121">无</span><span class="sxs-lookup"><span data-stu-id="20929-121">None</span></span>|<span data-ttu-id="20929-122">启用丢失模式</span><span class="sxs-lookup"><span data-stu-id="20929-122">Enable lost mode</span></span>|
|[<span data-ttu-id="20929-123">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="20929-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="20929-124">无</span><span class="sxs-lookup"><span data-stu-id="20929-124">None</span></span>|<span data-ttu-id="20929-125">远程锁定</span><span class="sxs-lookup"><span data-stu-id="20929-125">Remote lock</span></span>|
|[<span data-ttu-id="20929-126">setDeviceName 操作</span><span class="sxs-lookup"><span data-stu-id="20929-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="20929-127">无</span><span class="sxs-lookup"><span data-stu-id="20929-127">None</span></span>|<span data-ttu-id="20929-128">设置设备的设备名称。</span><span class="sxs-lookup"><span data-stu-id="20929-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="20929-129">rotateFileVaultKey 操作</span><span class="sxs-lookup"><span data-stu-id="20929-129">rotateFileVaultKey action</span></span>](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|<span data-ttu-id="20929-130">无</span><span class="sxs-lookup"><span data-stu-id="20929-130">None</span></span>|<span data-ttu-id="20929-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-131">Not yet documented</span></span>|
|[<span data-ttu-id="20929-132">getFileVaultKey 函数</span><span class="sxs-lookup"><span data-stu-id="20929-132">getFileVaultKey function</span></span>](../api/intune-devices-manageddevice-getfilevaultkey.md)|<span data-ttu-id="20929-133">字符串</span><span class="sxs-lookup"><span data-stu-id="20929-133">String</span></span>|<span data-ttu-id="20929-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-134">Not yet documented</span></span>|
|[<span data-ttu-id="20929-135">retire 操作</span><span class="sxs-lookup"><span data-stu-id="20929-135">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="20929-136">无</span><span class="sxs-lookup"><span data-stu-id="20929-136">None</span></span>|<span data-ttu-id="20929-137">停用设备</span><span class="sxs-lookup"><span data-stu-id="20929-137">Retire a device</span></span>|
|[<span data-ttu-id="20929-138">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="20929-138">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="20929-139">无</span><span class="sxs-lookup"><span data-stu-id="20929-139">None</span></span>|<span data-ttu-id="20929-140">擦除设备</span><span class="sxs-lookup"><span data-stu-id="20929-140">Wipe a device</span></span>|
|[<span data-ttu-id="20929-141">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="20929-141">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="20929-142">无</span><span class="sxs-lookup"><span data-stu-id="20929-142">None</span></span>|<span data-ttu-id="20929-143">重置密码</span><span class="sxs-lookup"><span data-stu-id="20929-143">Reset passcode</span></span>|
|[<span data-ttu-id="20929-144">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="20929-144">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="20929-145">无</span><span class="sxs-lookup"><span data-stu-id="20929-145">None</span></span>|<span data-ttu-id="20929-146">远程锁定</span><span class="sxs-lookup"><span data-stu-id="20929-146">Remote lock</span></span>|
|[<span data-ttu-id="20929-147">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="20929-147">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="20929-148">无</span><span class="sxs-lookup"><span data-stu-id="20929-148">None</span></span>|<span data-ttu-id="20929-149">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="20929-149">Request remote assistance</span></span>|
|[<span data-ttu-id="20929-150">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="20929-150">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="20929-151">无</span><span class="sxs-lookup"><span data-stu-id="20929-151">None</span></span>|<span data-ttu-id="20929-152">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="20929-152">Disable lost mode</span></span>|
|[<span data-ttu-id="20929-153">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="20929-153">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="20929-154">无</span><span class="sxs-lookup"><span data-stu-id="20929-154">None</span></span>|<span data-ttu-id="20929-155">查找设备</span><span class="sxs-lookup"><span data-stu-id="20929-155">Locate a device</span></span>|
|[<span data-ttu-id="20929-156">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="20929-156">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="20929-157">无</span><span class="sxs-lookup"><span data-stu-id="20929-157">None</span></span>|<span data-ttu-id="20929-158">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="20929-158">Bypass activation lock</span></span>|
|[<span data-ttu-id="20929-159">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="20929-159">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="20929-160">无</span><span class="sxs-lookup"><span data-stu-id="20929-160">None</span></span>|<span data-ttu-id="20929-161">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="20929-161">Reboot device</span></span>|
|[<span data-ttu-id="20929-162">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="20929-162">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="20929-163">无</span><span class="sxs-lookup"><span data-stu-id="20929-163">None</span></span>|<span data-ttu-id="20929-164">关闭设备</span><span class="sxs-lookup"><span data-stu-id="20929-164">Shut down device</span></span>|
|[<span data-ttu-id="20929-165">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="20929-165">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="20929-166">无</span><span class="sxs-lookup"><span data-stu-id="20929-166">None</span></span>|<span data-ttu-id="20929-167">恢复密码</span><span class="sxs-lookup"><span data-stu-id="20929-167">Recover passcode</span></span>|
|[<span data-ttu-id="20929-168">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="20929-168">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="20929-169">无</span><span class="sxs-lookup"><span data-stu-id="20929-169">None</span></span>|<span data-ttu-id="20929-170">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="20929-170">Clean Windows device</span></span>|
|[<span data-ttu-id="20929-171">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="20929-171">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="20929-172">无</span><span class="sxs-lookup"><span data-stu-id="20929-172">None</span></span>|<span data-ttu-id="20929-173">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="20929-173">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="20929-174">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="20929-174">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="20929-175">无</span><span class="sxs-lookup"><span data-stu-id="20929-175">None</span></span>|<span data-ttu-id="20929-176">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="20929-176">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="20929-177">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="20929-177">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="20929-178">无</span><span class="sxs-lookup"><span data-stu-id="20929-178">None</span></span>|<span data-ttu-id="20929-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-179">Not yet documented</span></span>|
|[<span data-ttu-id="20929-180">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="20929-180">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="20929-181">无</span><span class="sxs-lookup"><span data-stu-id="20929-181">None</span></span>|<span data-ttu-id="20929-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-182">Not yet documented</span></span>|
|[<span data-ttu-id="20929-183">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="20929-183">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="20929-184">无</span><span class="sxs-lookup"><span data-stu-id="20929-184">None</span></span>|<span data-ttu-id="20929-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-185">Not yet documented</span></span>|
|[<span data-ttu-id="20929-186">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="20929-186">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="20929-187">无</span><span class="sxs-lookup"><span data-stu-id="20929-187">None</span></span>|<span data-ttu-id="20929-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20929-188">Not yet documented</span></span>|
|[<span data-ttu-id="20929-189">revokeAppleVppLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="20929-189">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="20929-190">无</span><span class="sxs-lookup"><span data-stu-id="20929-190">None</span></span>|<span data-ttu-id="20929-191">吊销设备的所有 Apple Vpp 许可证</span><span class="sxs-lookup"><span data-stu-id="20929-191">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="20929-192">属性</span><span class="sxs-lookup"><span data-stu-id="20929-192">Properties</span></span>
|<span data-ttu-id="20929-193">属性</span><span class="sxs-lookup"><span data-stu-id="20929-193">Property</span></span>|<span data-ttu-id="20929-194">类型</span><span class="sxs-lookup"><span data-stu-id="20929-194">Type</span></span>|<span data-ttu-id="20929-195">说明</span><span class="sxs-lookup"><span data-stu-id="20929-195">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20929-196">id</span><span class="sxs-lookup"><span data-stu-id="20929-196">id</span></span>|<span data-ttu-id="20929-197">字符串</span><span class="sxs-lookup"><span data-stu-id="20929-197">String</span></span>|<span data-ttu-id="20929-198">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="20929-198">Unique Identifier for the device</span></span>|
|<span data-ttu-id="20929-199">userId</span><span class="sxs-lookup"><span data-stu-id="20929-199">userId</span></span>|<span data-ttu-id="20929-200">String</span><span class="sxs-lookup"><span data-stu-id="20929-200">String</span></span>|<span data-ttu-id="20929-201">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="20929-201">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="20929-202">deviceName</span><span class="sxs-lookup"><span data-stu-id="20929-202">deviceName</span></span>|<span data-ttu-id="20929-203">String</span><span class="sxs-lookup"><span data-stu-id="20929-203">String</span></span>|<span data-ttu-id="20929-204">设备的名称</span><span class="sxs-lookup"><span data-stu-id="20929-204">Name of the device</span></span>|
|<span data-ttu-id="20929-205">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="20929-205">hardwareInformation</span></span>|[<span data-ttu-id="20929-206">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="20929-206">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="20929-207">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="20929-207">The hardward details for the device.</span></span>  <span data-ttu-id="20929-208">包括存储空间、制造商、序列号等信息。</span><span class="sxs-lookup"><span data-stu-id="20929-208">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="20929-209">所有者</span><span class="sxs-lookup"><span data-stu-id="20929-209">ownerType</span></span>|[<span data-ttu-id="20929-210">所有者</span><span class="sxs-lookup"><span data-stu-id="20929-210">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="20929-211">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="20929-211">Ownership of the device.</span></span> <span data-ttu-id="20929-212">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="20929-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="20929-213">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="20929-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="20929-214">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="20929-214">managedDeviceOwnerType</span></span>|[<span data-ttu-id="20929-215">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="20929-215">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="20929-216">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="20929-216">Ownership of the device.</span></span> <span data-ttu-id="20929-217">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="20929-217">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="20929-218">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="20929-218">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="20929-219">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="20929-219">deviceActionResults</span></span>|<span data-ttu-id="20929-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20929-220">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="20929-221">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="20929-221">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="20929-222">managementState</span><span class="sxs-lookup"><span data-stu-id="20929-222">managementState</span></span>|[<span data-ttu-id="20929-223">managementState</span><span class="sxs-lookup"><span data-stu-id="20929-223">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="20929-224">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="20929-224">Management state of the device.</span></span> <span data-ttu-id="20929-225">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="20929-225">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="20929-226">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-226">enrolledDateTime</span></span>|<span data-ttu-id="20929-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-227">DateTimeOffset</span></span>|<span data-ttu-id="20929-228">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="20929-228">Enrollment time of the device.</span></span>|
|<span data-ttu-id="20929-229">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-229">lastSyncDateTime</span></span>|<span data-ttu-id="20929-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-230">DateTimeOffset</span></span>|<span data-ttu-id="20929-231">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="20929-231">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="20929-232">chassisType</span><span class="sxs-lookup"><span data-stu-id="20929-232">chassisType</span></span>|[<span data-ttu-id="20929-233">chassisType</span><span class="sxs-lookup"><span data-stu-id="20929-233">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="20929-234">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="20929-234">Chassis type of the device.</span></span> <span data-ttu-id="20929-235">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="20929-235">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="20929-236">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="20929-236">operatingSystem</span></span>|<span data-ttu-id="20929-237">String</span><span class="sxs-lookup"><span data-stu-id="20929-237">String</span></span>|<span data-ttu-id="20929-238">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="20929-238">Operating system of the device.</span></span> <span data-ttu-id="20929-239">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="20929-239">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="20929-240">deviceType</span><span class="sxs-lookup"><span data-stu-id="20929-240">deviceType</span></span>|[<span data-ttu-id="20929-241">deviceType</span><span class="sxs-lookup"><span data-stu-id="20929-241">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="20929-242">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="20929-242">Platform of the device.</span></span> <span data-ttu-id="20929-243">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="20929-243">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="20929-244">complianceState</span><span class="sxs-lookup"><span data-stu-id="20929-244">complianceState</span></span>|[<span data-ttu-id="20929-245">complianceState</span><span class="sxs-lookup"><span data-stu-id="20929-245">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="20929-246">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="20929-246">Compliance state of the device.</span></span> <span data-ttu-id="20929-247">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="20929-247">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="20929-248">jailBroken</span><span class="sxs-lookup"><span data-stu-id="20929-248">jailBroken</span></span>|<span data-ttu-id="20929-249">String</span><span class="sxs-lookup"><span data-stu-id="20929-249">String</span></span>|<span data-ttu-id="20929-250">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="20929-250">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="20929-251">managementAgent</span><span class="sxs-lookup"><span data-stu-id="20929-251">managementAgent</span></span>|[<span data-ttu-id="20929-252">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="20929-252">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="20929-253">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="20929-253">Management channel of the device.</span></span> <span data-ttu-id="20929-254">Intune、EAS 等。可能的值为`eas`: `mdm`、 `easMdm`、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`、、、、、、、、 `microsoft365ManagedMdm` `jamf` `googleCloudDevicePolicyController`</span><span class="sxs-lookup"><span data-stu-id="20929-254">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="20929-255">osVersion</span><span class="sxs-lookup"><span data-stu-id="20929-255">osVersion</span></span>|<span data-ttu-id="20929-256">String</span><span class="sxs-lookup"><span data-stu-id="20929-256">String</span></span>|<span data-ttu-id="20929-257">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="20929-257">Operating system version of the device.</span></span>|
|<span data-ttu-id="20929-258">easActivated</span><span class="sxs-lookup"><span data-stu-id="20929-258">easActivated</span></span>|<span data-ttu-id="20929-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-259">Boolean</span></span>|<span data-ttu-id="20929-260">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="20929-260">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="20929-261">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="20929-261">easDeviceId</span></span>|<span data-ttu-id="20929-262">String</span><span class="sxs-lookup"><span data-stu-id="20929-262">String</span></span>|<span data-ttu-id="20929-263">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="20929-263">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="20929-264">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-264">easActivationDateTime</span></span>|<span data-ttu-id="20929-265">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-265">DateTimeOffset</span></span>|<span data-ttu-id="20929-266">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="20929-266">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="20929-267">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="20929-267">aadRegistered</span></span>|<span data-ttu-id="20929-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-268">Boolean</span></span>|<span data-ttu-id="20929-269">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="20929-269">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="20929-270">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="20929-270">azureADRegistered</span></span>|<span data-ttu-id="20929-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-271">Boolean</span></span>|<span data-ttu-id="20929-272">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="20929-272">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="20929-273">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="20929-273">deviceEnrollmentType</span></span>|[<span data-ttu-id="20929-274">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="20929-274">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="20929-275">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="20929-275">Enrollment type of the device.</span></span> <span data-ttu-id="20929-276">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="20929-276">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="20929-277">lostModeState</span><span class="sxs-lookup"><span data-stu-id="20929-277">lostModeState</span></span>|[<span data-ttu-id="20929-278">lostModeState</span><span class="sxs-lookup"><span data-stu-id="20929-278">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="20929-279">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="20929-279">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="20929-280">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="20929-280">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="20929-281">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="20929-281">activationLockBypassCode</span></span>|<span data-ttu-id="20929-282">String</span><span class="sxs-lookup"><span data-stu-id="20929-282">String</span></span>|<span data-ttu-id="20929-283">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="20929-283">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="20929-284">emailAddress</span><span class="sxs-lookup"><span data-stu-id="20929-284">emailAddress</span></span>|<span data-ttu-id="20929-285">String</span><span class="sxs-lookup"><span data-stu-id="20929-285">String</span></span>|<span data-ttu-id="20929-286">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="20929-286">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="20929-287">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="20929-287">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="20929-288">String</span><span class="sxs-lookup"><span data-stu-id="20929-288">String</span></span>|<span data-ttu-id="20929-289">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="20929-289">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="20929-290">只读。</span><span class="sxs-lookup"><span data-stu-id="20929-290">Read only.</span></span>|
|<span data-ttu-id="20929-291">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="20929-291">azureADDeviceId</span></span>|<span data-ttu-id="20929-292">String</span><span class="sxs-lookup"><span data-stu-id="20929-292">String</span></span>|<span data-ttu-id="20929-293">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="20929-293">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="20929-294">只读。</span><span class="sxs-lookup"><span data-stu-id="20929-294">Read only.</span></span>|
|<span data-ttu-id="20929-295">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="20929-295">deviceRegistrationState</span></span>|[<span data-ttu-id="20929-296">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="20929-296">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="20929-297">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="20929-297">Device registration state.</span></span> <span data-ttu-id="20929-298">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="20929-298">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="20929-299">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="20929-299">deviceCategoryDisplayName</span></span>|<span data-ttu-id="20929-300">String</span><span class="sxs-lookup"><span data-stu-id="20929-300">String</span></span>|<span data-ttu-id="20929-301">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="20929-301">Device category display name</span></span>|
|<span data-ttu-id="20929-302">isSupervised</span><span class="sxs-lookup"><span data-stu-id="20929-302">isSupervised</span></span>|<span data-ttu-id="20929-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-303">Boolean</span></span>|<span data-ttu-id="20929-304">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="20929-304">Device supervised status</span></span>|
|<span data-ttu-id="20929-305">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-305">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="20929-306">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-306">DateTimeOffset</span></span>|<span data-ttu-id="20929-307">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="20929-307">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="20929-308">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="20929-308">exchangeAccessState</span></span>|[<span data-ttu-id="20929-309">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="20929-309">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="20929-310">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="20929-310">The Access State of the device in Exchange.</span></span> <span data-ttu-id="20929-311">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="20929-311">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="20929-312">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="20929-312">exchangeAccessStateReason</span></span>|[<span data-ttu-id="20929-313">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="20929-313">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="20929-314">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="20929-314">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="20929-315">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="20929-315">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="20929-316">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="20929-316">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="20929-317">String</span><span class="sxs-lookup"><span data-stu-id="20929-317">String</span></span>|<span data-ttu-id="20929-318">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="20929-318">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="20929-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="20929-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="20929-320">String</span><span class="sxs-lookup"><span data-stu-id="20929-320">String</span></span>|<span data-ttu-id="20929-321">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="20929-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="20929-322">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="20929-322">isEncrypted</span></span>|<span data-ttu-id="20929-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-323">Boolean</span></span>|<span data-ttu-id="20929-324">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="20929-324">Device encryption status</span></span>|
|<span data-ttu-id="20929-325">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20929-325">userPrincipalName</span></span>|<span data-ttu-id="20929-326">字符串</span><span class="sxs-lookup"><span data-stu-id="20929-326">String</span></span>|<span data-ttu-id="20929-327">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="20929-327">Device user principal name</span></span>|
|<span data-ttu-id="20929-328">model</span><span class="sxs-lookup"><span data-stu-id="20929-328">model</span></span>|<span data-ttu-id="20929-329">String</span><span class="sxs-lookup"><span data-stu-id="20929-329">String</span></span>|<span data-ttu-id="20929-330">设备的型号</span><span class="sxs-lookup"><span data-stu-id="20929-330">Model of the device</span></span>|
|<span data-ttu-id="20929-331">manufacturer</span><span class="sxs-lookup"><span data-stu-id="20929-331">manufacturer</span></span>|<span data-ttu-id="20929-332">String</span><span class="sxs-lookup"><span data-stu-id="20929-332">String</span></span>|<span data-ttu-id="20929-333">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="20929-333">Manufacturer of the device</span></span>|
|<span data-ttu-id="20929-334">imei</span><span class="sxs-lookup"><span data-stu-id="20929-334">imei</span></span>|<span data-ttu-id="20929-335">String</span><span class="sxs-lookup"><span data-stu-id="20929-335">String</span></span>|<span data-ttu-id="20929-336">IMEI</span><span class="sxs-lookup"><span data-stu-id="20929-336">IMEI</span></span>|
|<span data-ttu-id="20929-337">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-337">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="20929-338">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-338">DateTimeOffset</span></span>|<span data-ttu-id="20929-339">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="20929-339">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="20929-340">serialNumber</span><span class="sxs-lookup"><span data-stu-id="20929-340">serialNumber</span></span>|<span data-ttu-id="20929-341">字符串</span><span class="sxs-lookup"><span data-stu-id="20929-341">String</span></span>|<span data-ttu-id="20929-342">序列号</span><span class="sxs-lookup"><span data-stu-id="20929-342">SerialNumber</span></span>|
|<span data-ttu-id="20929-343">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="20929-343">phoneNumber</span></span>|<span data-ttu-id="20929-344">String</span><span class="sxs-lookup"><span data-stu-id="20929-344">String</span></span>|<span data-ttu-id="20929-345">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="20929-345">Phone number of the device</span></span>|
|<span data-ttu-id="20929-346">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="20929-346">androidSecurityPatchLevel</span></span>|<span data-ttu-id="20929-347">String</span><span class="sxs-lookup"><span data-stu-id="20929-347">String</span></span>|<span data-ttu-id="20929-348">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="20929-348">Android security patch level</span></span>|
|<span data-ttu-id="20929-349">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="20929-349">userDisplayName</span></span>|<span data-ttu-id="20929-350">String</span><span class="sxs-lookup"><span data-stu-id="20929-350">String</span></span>|<span data-ttu-id="20929-351">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="20929-351">User display name</span></span>|
|<span data-ttu-id="20929-352">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="20929-352">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="20929-353">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="20929-353">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="20929-354">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="20929-354">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="20929-355">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="20929-355">wiFiMacAddress</span></span>|<span data-ttu-id="20929-356">String</span><span class="sxs-lookup"><span data-stu-id="20929-356">String</span></span>|<span data-ttu-id="20929-357">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="20929-357">Wi-Fi MAC</span></span>|
|<span data-ttu-id="20929-358">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="20929-358">deviceHealthAttestationState</span></span>|[<span data-ttu-id="20929-359">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="20929-359">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="20929-360">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="20929-360">The device health attestation state.</span></span>|
|<span data-ttu-id="20929-361">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="20929-361">subscriberCarrier</span></span>|<span data-ttu-id="20929-362">String</span><span class="sxs-lookup"><span data-stu-id="20929-362">String</span></span>|<span data-ttu-id="20929-363">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="20929-363">Subscriber Carrier</span></span>|
|<span data-ttu-id="20929-364">meid</span><span class="sxs-lookup"><span data-stu-id="20929-364">meid</span></span>|<span data-ttu-id="20929-365">String</span><span class="sxs-lookup"><span data-stu-id="20929-365">String</span></span>|<span data-ttu-id="20929-366">MEID</span><span class="sxs-lookup"><span data-stu-id="20929-366">MEID</span></span>|
|<span data-ttu-id="20929-367">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="20929-367">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="20929-368">Int64</span><span class="sxs-lookup"><span data-stu-id="20929-368">Int64</span></span>|<span data-ttu-id="20929-369">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="20929-369">Total Storage in Bytes</span></span>|
|<span data-ttu-id="20929-370">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="20929-370">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="20929-371">Int64</span><span class="sxs-lookup"><span data-stu-id="20929-371">Int64</span></span>|<span data-ttu-id="20929-372">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="20929-372">Free Storage in Bytes</span></span>|
|<span data-ttu-id="20929-373">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="20929-373">managedDeviceName</span></span>|<span data-ttu-id="20929-374">String</span><span class="sxs-lookup"><span data-stu-id="20929-374">String</span></span>|<span data-ttu-id="20929-375">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="20929-375">Automatically generated name to identify a device.</span></span> <span data-ttu-id="20929-376">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="20929-376">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="20929-377">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="20929-377">partnerReportedThreatState</span></span>|[<span data-ttu-id="20929-378">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="20929-378">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="20929-379">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="20929-379">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="20929-380">只读。</span><span class="sxs-lookup"><span data-stu-id="20929-380">Read Only.</span></span> <span data-ttu-id="20929-381">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="20929-381">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="20929-382">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-382">retireAfterDateTime</span></span>|<span data-ttu-id="20929-383">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-383">DateTimeOffset</span></span>|<span data-ttu-id="20929-384">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="20929-384">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="20929-385">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="20929-385">usersLoggedOn</span></span>|<span data-ttu-id="20929-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="20929-386">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="20929-387">指示设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="20929-387">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="20929-388">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="20929-388">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="20929-389">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-389">DateTimeOffset</span></span>|<span data-ttu-id="20929-390">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="20929-390">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="20929-391">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="20929-391">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="20929-392">只读。</span><span class="sxs-lookup"><span data-stu-id="20929-392">Read Only.</span></span>|
|<span data-ttu-id="20929-393">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="20929-393">autopilotEnrolled</span></span>|<span data-ttu-id="20929-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-394">Boolean</span></span>|<span data-ttu-id="20929-395">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="20929-395">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="20929-396">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="20929-396">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="20929-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="20929-397">Boolean</span></span>|<span data-ttu-id="20929-398">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="20929-398">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="20929-399">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="20929-399">managementCertificateExpirationDate</span></span>|<span data-ttu-id="20929-400">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20929-400">DateTimeOffset</span></span>|<span data-ttu-id="20929-401">报告设备管理证书到期日期</span><span class="sxs-lookup"><span data-stu-id="20929-401">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="20929-402">iccid</span><span class="sxs-lookup"><span data-stu-id="20929-402">iccid</span></span>|<span data-ttu-id="20929-403">String</span><span class="sxs-lookup"><span data-stu-id="20929-403">String</span></span>|<span data-ttu-id="20929-404">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="20929-404">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="20929-405">udid</span><span class="sxs-lookup"><span data-stu-id="20929-405">udid</span></span>|<span data-ttu-id="20929-406">String</span><span class="sxs-lookup"><span data-stu-id="20929-406">String</span></span>|<span data-ttu-id="20929-407">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="20929-407">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="20929-408">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20929-408">roleScopeTagIds</span></span>|<span data-ttu-id="20929-409">String collection</span><span class="sxs-lookup"><span data-stu-id="20929-409">String collection</span></span>|<span data-ttu-id="20929-410">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="20929-410">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="20929-411">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="20929-411">windowsActiveMalwareCount</span></span>|<span data-ttu-id="20929-412">Int32</span><span class="sxs-lookup"><span data-stu-id="20929-412">Int32</span></span>|<span data-ttu-id="20929-413">此 windows 设备的活动恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="20929-413">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="20929-414">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="20929-414">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="20929-415">Int32</span><span class="sxs-lookup"><span data-stu-id="20929-415">Int32</span></span>|<span data-ttu-id="20929-416">此 windows 设备的修正的恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="20929-416">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="20929-417">notes</span><span class="sxs-lookup"><span data-stu-id="20929-417">notes</span></span>|<span data-ttu-id="20929-418">String</span><span class="sxs-lookup"><span data-stu-id="20929-418">String</span></span>|<span data-ttu-id="20929-419">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="20929-419">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="20929-420">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="20929-420">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="20929-421">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="20929-421">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="20929-422">Configuration manager 客户端运行状况状态, 仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="20929-422">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="20929-423">关系</span><span class="sxs-lookup"><span data-stu-id="20929-423">Relationships</span></span>
|<span data-ttu-id="20929-424">关系</span><span class="sxs-lookup"><span data-stu-id="20929-424">Relationship</span></span>|<span data-ttu-id="20929-425">类型</span><span class="sxs-lookup"><span data-stu-id="20929-425">Type</span></span>|<span data-ttu-id="20929-426">说明</span><span class="sxs-lookup"><span data-stu-id="20929-426">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20929-427">detectedApps</span><span class="sxs-lookup"><span data-stu-id="20929-427">detectedApps</span></span>|<span data-ttu-id="20929-428">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20929-428">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="20929-429">设备上当前安装的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="20929-429">All applications currently installed on the device</span></span>|
|<span data-ttu-id="20929-430">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="20929-430">deviceCategory</span></span>|[<span data-ttu-id="20929-431">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="20929-431">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="20929-432">设备类别</span><span class="sxs-lookup"><span data-stu-id="20929-432">Device category</span></span>|
|<span data-ttu-id="20929-433">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="20929-433">windowsProtectionState</span></span>|[<span data-ttu-id="20929-434">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="20929-434">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="20929-435">设备保护状态。</span><span class="sxs-lookup"><span data-stu-id="20929-435">The device protection status.</span></span>|
|<span data-ttu-id="20929-436">users</span><span class="sxs-lookup"><span data-stu-id="20929-436">users</span></span>|<span data-ttu-id="20929-437">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20929-437">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="20929-438">与托管设备关联的主要用户。</span><span class="sxs-lookup"><span data-stu-id="20929-438">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20929-439">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20929-439">JSON Representation</span></span>
<span data-ttu-id="20929-440">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20929-440">Here is a JSON representation of the resource.</span></span>
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
  "retireAfterDateTime": "String (timestamp)",
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





