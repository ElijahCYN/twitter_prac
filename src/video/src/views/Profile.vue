<template>
    <div>
        <header class="profile container">
            <div class="profile-container grid">
                <div class="profile-data">
                    <div class="profile-border">
                        <div class="profile-perfil">
                            <img src="../assets/img/IMG_0278.jpg" alt="" />
                        </div>
                    </div>
                    <h2 class="profile-name">Elijah Chang</h2>
                    <h3 class="profile-profession">Soft engineer</h3>

                    <ul class="profile-social">
                        <a
                            href="https://www.instagram.com/"
                            target="_blank"
                            class="profile-social-link"
                        >
                            <i class="ri-instagram-line"></i>
                        </a>
                        <a
                            href="https://www.linkedin.com/"
                            target="_blank"
                            class="profile-social-link"
                        >
                            <i class="ri-linkedin-box-line"></i>
                        </a>
                        <a
                            href="https://github.com/"
                            target="_blank"
                            class="profile-social-link"
                        >
                            <i class="ri-github-fill"></i>
                        </a>
                    </ul>
                </div>

                <div class="profile-info grid">
                    <div class="profile-info-group">
                        <h3 class="profile-info-number">7</h3>
                        <p class="profile-info-description">
                            Years of <br />
                            work
                        </p>
                    </div>
                    <div class="profile-info-group">
                        <h3 class="profile-info-number">+124</h3>
                        <p class="profile-info-description">
                            Completed <br />
                            projects
                        </p>
                    </div>
                    <div class="profile-info-group">
                        <h3 class="profile-info-number">96</h3>
                        <p class="profile-info-description">
                            Satisfied <br />
                            customers
                        </p>
                    </div>
                </div>

                <div class="profile-buttons">
                    <a href="" download="" class="button">
                        Download CV <i class="ri-download-line"></i>
                    </a>
                    <div class="profile-buttons-small">
                        <a
                            href=""
                            target="_blank"
                            class="button button-small button-gray"
                        >
                            <i class="ri-messenger-line"></i>
                        </a>
                    </div>
                </div>
            </div>
        </header>

        <main class="main">
            <section class="filters container">
                <ul class="filters-content">
                    <button class="filters-button" data-target="#projects">
                        Projects
                    </button>
                    <button class="filters-button" data-target="#skills">
                        Skills
                    </button>
                </ul>
                <div class="filters-sections">
                    <div
                        id="projects"
                        class="projects-content grid"
                        data-content
                    >
                        <article class="projects-card">
                            <img
                                src="../assets/img/edgar-moran.jpg"
                                alt=""
                                class="projects-img"
                            />
                            <div class="projects-modal">
                                <div>
                                    <span class="projects-subtitle">Web</span>
                                    <h3 class="projects-title">Payment Site</h3>
                                    <a
                                        href="#"
                                        class="projects-button button button-small"
                                    >
                                        <i class="ri-link"></i>
                                    </a>
                                </div>
                            </div>
                        </article>
                        <article class="projects-card">
                            <img
                                src="../assets/img/edgar-moran.jpg"
                                alt=""
                                class="projects-img"
                            />
                            <div class="projects-modal">
                                <div>
                                    <span class="projects-subtitle">Web</span>
                                    <h3 class="projects-title">Payment Site</h3>
                                    <a
                                        href="#"
                                        class="projects-button button button-small"
                                    >
                                        <i class="ri-link"></i>
                                    </a>
                                </div>
                            </div>
                        </article>
                        <article class="projects-card">
                            <img
                                src="../assets/img/edgar-moran.jpg"
                                alt=""
                                class="projects-img"
                            />
                            <div class="projects-modal">
                                <div>
                                    <span class="projects-subtitle">Web</span>
                                    <h3 class="projects-title">Payment Site</h3>
                                    <a
                                        href="#"
                                        class="projects-button button button-small"
                                    >
                                        <i class="ri-link"></i>
                                    </a>
                                </div>
                            </div>
                        </article>
                        <article class="projects-card">
                            <img
                                src="../assets/img/edgar-moran.jpg"
                                alt=""
                                class="projects-img"
                            />
                            <div class="projects-modal">
                                <div>
                                    <span class="projects-subtitle">Web</span>
                                    <h3 class="projects-title">Payment Site</h3>
                                    <a
                                        href="#"
                                        class="projects-button button button-small"
                                    >
                                        <i class="ri-link"></i>
                                    </a>
                                </div>
                            </div>
                        </article>
                        <article class="projects-card">
                            <img
                                src="../assets/img/edgar-moran.jpg"
                                alt=""
                                class="projects-img"
                            />
                            <div class="projects-modal">
                                <div>
                                    <span class="projects-subtitle">Web</span>
                                    <h3 class="projects-title">Payment Site</h3>
                                    <a
                                        href="#"
                                        class="projects-button button button-small"
                                    >
                                        <i class="ri-link"></i>
                                    </a>
                                </div>
                            </div>
                        </article>
                    </div>
                    <div id="skills" class="skills-content grid" data-content>
                        <div class="skills-area"></div>
                    </div>
                </div>
            </section>
        </main>
        <!-- <div class="profile-avatar">
      <el-upload
        class="avatar-uploader"
        :action="uploadUrl"
        :headers="headers"
        name="image"
        :show-file-list="false"
        :on-success="handleAvatarSuccess"
        :before-upload="beforeAvatarUpload"
      >
        <el-avatar
          v-if="profile.avatar != ''"
          :src="imgUrl + profile.avatar"
          fit="fill"
        ></el-avatar>
        <i class="ri-upload-line" v-else></i>
      </el-upload>
    </div> -->

        <!-- <div class="profile-content">
      <el-row :gutter="12" justify="center">
        <el-col :offset="4" :span="5">
          <span>UserName </span>
        </el-col>
        <el-col :span="6">
          <span> {{ profile.user_id }}</span>
        </el-col>
      </el-row>

      <el-row :gutter="12" justify="center">
        <el-col :offset="4" :span="5">
          <span>Email </span>
        </el-col>
        <el-col :span="6">
          <span>123</span>
        </el-col>
      </el-row>
    </div> -->
    </div>
</template>

<script>
import axios from "axios";
import api from "../common/api";

export default {
    data() {
        return {
            imgUrl: api.main.getImg,
            uploadUrl: api.main.avatar,
            headers: axios.defaults.headers.common,
            profile: {
                avatar: "",
            },
            img: "",
            image: "",
        };
    },
    methods: {
        getProfile() {
            let me = this;
            axios.get(api.main.profile).then(function (response) {
                if (response.data.Code == 200) {
                    me.profile = response.data.Data;
                } else {
                    alert(response.data.Msg);
                }
            });
        },

        beforeAvatarUpload() {
            console.log("before");
            return true;
        },

        handleAvatarSuccess() {
            console.log("handle");
        },

        test(event) {
            console.log(event);
        },
    },
    mounted() {
        this.getProfile();
    },
};
</script>
