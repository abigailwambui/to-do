--
-- PostgreSQL database dump
--

-- Dumped from database version 10.8 (Ubuntu 10.8-0ubuntu0.18.10.1)
-- Dumped by pg_dump version 10.8 (Ubuntu 10.8-0ubuntu0.18.10.1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

--
-- Name: plpgsql; Type: EXTENSION; Schema: -; Owner: 
--

CREATE EXTENSION IF NOT EXISTS plpgsql WITH SCHEMA pg_catalog;


--
-- Name: EXTENSION plpgsql; Type: COMMENT; Schema: -; Owner: 
--

COMMENT ON EXTENSION plpgsql IS 'PL/pgSQL procedural language';


SET default_tablespace = '';

SET default_with_oids = false;

--
-- Name: categories; Type: TABLE; Schema: public; Owner: abigail
--

CREATE TABLE public.categories (
    id integer NOT NULL,
    name character varying
);


ALTER TABLE public.categories OWNER TO abigail;

--
-- Name: categories_id_seq; Type: SEQUENCE; Schema: public; Owner: abigail
--

CREATE SEQUENCE public.categories_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.categories_id_seq OWNER TO abigail;

--
-- Name: categories_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: abigail
--

ALTER SEQUENCE public.categories_id_seq OWNED BY public.categories.id;


--
-- Name: tasks; Type: TABLE; Schema: public; Owner: abigail
--

CREATE TABLE public.tasks (
    id integer NOT NULL,
    description character varying,
    categoryid integer
);


ALTER TABLE public.tasks OWNER TO abigail;

--
-- Name: tasks_id_seq; Type: SEQUENCE; Schema: public; Owner: abigail
--

CREATE SEQUENCE public.tasks_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.tasks_id_seq OWNER TO abigail;

--
-- Name: tasks_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: abigail
--

ALTER SEQUENCE public.tasks_id_seq OWNED BY public.tasks.id;


--
-- Name: categories id; Type: DEFAULT; Schema: public; Owner: abigail
--

ALTER TABLE ONLY public.categories ALTER COLUMN id SET DEFAULT nextval('public.categories_id_seq'::regclass);


--
-- Name: tasks id; Type: DEFAULT; Schema: public; Owner: abigail
--

ALTER TABLE ONLY public.tasks ALTER COLUMN id SET DEFAULT nextval('public.tasks_id_seq'::regclass);


--
-- Data for Name: categories; Type: TABLE DATA; Schema: public; Owner: abigail
--

COPY public.categories (id, name) FROM stdin;
1	Abigail Wambui
2	Abigail Wambui
3	x
4	
5	
\.


--
-- Data for Name: tasks; Type: TABLE DATA; Schema: public; Owner: abigail
--

COPY public.tasks (id, description, categoryid) FROM stdin;
5	Clean kitchen	3
6	Clean kitchen	3
7	Clean kitchen	3
4	gggggg	3
2	Blogging	1
\.


--
-- Name: categories_id_seq; Type: SEQUENCE SET; Schema: public; Owner: abigail
--

SELECT pg_catalog.setval('public.categories_id_seq', 5, true);


--
-- Name: tasks_id_seq; Type: SEQUENCE SET; Schema: public; Owner: abigail
--

SELECT pg_catalog.setval('public.tasks_id_seq', 9, true);


--
-- Name: categories categories_pkey; Type: CONSTRAINT; Schema: public; Owner: abigail
--

ALTER TABLE ONLY public.categories
    ADD CONSTRAINT categories_pkey PRIMARY KEY (id);


--
-- Name: tasks tasks_pkey; Type: CONSTRAINT; Schema: public; Owner: abigail
--

ALTER TABLE ONLY public.tasks
    ADD CONSTRAINT tasks_pkey PRIMARY KEY (id);


--
-- PostgreSQL database dump complete
--

